---
title: "Ray Tracer Vol5"
layout: post
date: 2017-04-20 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the fifth step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 5 </center>
<center>
<p>
This is the fifth step of my Ray Tracer homework. This week, there are many new things which include 
multisampling, depth of field, metalic-looking surfaces, area lights and spot lights. 
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p align="center">
  <img src="../assets/images/5/dragon_spot_light.png" alt="Dragon Spot Light"/>
  <figcaption>Dragon Spot Light</figcaption>
</p>
<center>

<p>
This image shows the output of the spot light effect. It creates a fully illuminated region, as well
 as soft shadows surrounding it. This effect creates more realistic shadows, rather than so perfectly 
 drawn shadows. But as you can see, the results are too digital, the square shapes around the shadow 
 of the dragon makes the image look too digital. At this point, it was time to implement multi-sampling. 
 This image takes around a second to render.
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/dragon_spot_light.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/5/dragon_spot_light_msaa.png" alt="Dragon Spot Light"/>
  <figcaption>Dragon Spot Light with Multisampling</figcaption>
</p>

<center>
<p>
Here, you can see the effect of multisampling. All those rectangles are gone, creating a more smooth shadow.
Of course this procedure dramatically increases the running time of my ray tracer with the number of samples 
linearly. This image took around 80 seconds for 100 samples per pixel.
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/dragon_spot_light_msaa.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/5/glass_plates_area.png" alt="Area Light"/>
  <figcaption>Area Light</figcaption>
</p>

<center>
<p>
This scene contains the previous glass plates, but now it has area light. The implementation of an area light
introduced soft shadows as well. This scene took 150 seconds for 36 samples. 
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/glass_plates_area.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/5/glass_plates_point.png" alt="Glass Plates"/>
  <figcaption>Glass Plates</figcaption>
</p>

<center>
<p>
This is the point light version of the previous scene. You can see the difference of adding area light here. 
This scene took around 140 seconds with the same 36 samples, which is almost the same as the area-lighted version.
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/glass_plates_point.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/5/metal_plates_area.png" alt="Metal Plates"/>
  <figcaption>Metal Plates</figcaption>
</p>

<center>
<p>
This image shows the effect of metalic surfaces, combined with area ligths. It also took almost the same amount
of time as the previosu two versions with the same amount of samples.
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/metal_plates_area.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/5/spheres_dof.png" alt="Depth of Field"/>
  <figcaption>Depth of Field</figcaption>
</p>

<center>
<p>
And now, the natural effect of adding multisampling (with a little modification) can be seen in this input. For
the depth of field effect, we only move the image plane forward, to the point where we want to focus. This way
we have the blurred effect, but the running time is almost 10 minutes, with 100 samples per pixel.
</p>
<p>
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/5/spheres_dof.xml">here</a>.
</p>
</center>


<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
