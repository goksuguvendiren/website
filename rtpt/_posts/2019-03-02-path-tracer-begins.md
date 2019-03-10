---
title: "Basic Path Tracer"
layout: post
date: 2019-03-02 11.00
tag: path tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the basic path tracer, only lambertian materials are used.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---

## GPU Path Tracer

This is the initial state of my path tracer. Actually, this is almost the same thing that comes with the nVidia's 
OptiX SDK. The output of a cornell box looks like this:

<p align="center">
<img src ="../assets/images/output10.png" />
</p>
In this scene, there is a single parallelogram light source. All the materials are lambertian, and rays are terminated according
to russian roulette. 

In this project, I'll be learning how to use the OptiX SDK while implementing a path tracer. 

### Writing the ray generation for a pinhole camera, with lambertian surfaces.

Here it comes. I will explain how to write the shader for a basic ray tracer, with a pinhole camera model. For that, we 
create a cuda file, and write the ray generation program inside it. For this case, I named it "ray_tracer.cu", and the 
function name is "pinhole_camera". 

First thing to do is to let the OptiX know that the ray generation program will be inside ray_tracer.cu, named as pinhole_camera.

```cpp
const char *ptx = sutil::getPtxString( sc.sample_name.c_str(), "../src/ray_generators/ray_tracer.cu" );
context->setRayGenerationProgram( 0, context->createProgramFromPTXString( ptx, "pinhole_camera" ) );
```

Now, we can actually move onto the ray generation program. In the ray_tracer.cu file, I create a regular function with 
the only difference that I have to mark this function as an optix program. I do this by putting the keyword RT_PROGRAM
to the beginning of the function declaration:

```cpp
RT_PROGRAM void pinhole_camera()
{
    ...
}
```

Now, moving onto the basic ray tracing. First, I get the size of my output buffer (will be the buffer where I will put the
color information for each pixel) with the line :

```cpp
size_t2 screen = output_buffer.size();
```

This gives me the width and height of the output image, actually. Now, I need to create an actual ray to send into the 
scene. The origin of the ray will be the camera's position. The direction will be the center of the pixel:
```cpp
float2 d = make_float2(launch_index) / make_float2(screen) * 2.f - 1.f;
float3 ray_origin = eye;
float3 ray_direction = normalize(d.x*U + d.y*V + W);
```

We are ready to create and send the ray! 

```cpp
Ray ray = make_Ray(ray_origin, ray_direction, pathtrace_ray_type, scene_epsilon, RT_DEFAULT_MAX);
rtTrace(top_object, ray, prd);
```

Here, the pathtracer_ray_type is the enumeration of the ray type. For primary rays, it is 0. For secondary rays (such as
shadow rays), it is set to 1. There can be more types of rays, though. Scene epsilon is used as the minimum distance of 
an intersection, and RT_DEFAULT_MAX is the maximum distance that a hit can happen.

rtTrace function is where the actual ray tracing happens. top_object is the scene geometry, and the prd is the data that 
is filled in other parts of execution that we will discuss.

After that, assuming that the prd.result is the component that has the color information for the current pixel, we can set
it to the output buffer, and be done with the ray!

```cpp
output_buffer[launch_index] = make_float4(prd.result, 1.0f);
```

The GitHub link to this version is [here](https://github.com/goksuguvendiren/optix_renderer/releases/tag/v0.0)