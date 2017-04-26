---
title: "Ray Tracer Vol6"
layout: post
date: 2017-04-25 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the sixth step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 6 </center>
<center>
<p>
This is the sixth step of my Ray Tracer homework. This week I have added texture mapping, and perlin noise support.
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p align="center">
  <img src="../assets/images/6/simple_texture.png" alt="Simple Texture Mapping"/>
  <figcaption>Texture Mapping Basics</figcaption>
</p>
<center>

<p>
This image is the basics of texture mapping and perlin noise. You can see texture mapping on spheres, triangles,
and meshes. Perlin noise types Vein and Patch can also be seen in spheres in lower left and right of the image.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/simple_texture.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/6/sphere_texture_blend_bilinear.png" alt="Bilinear Texture Blending"/>
  <figcaption>Bilinear Texture Blending</figcaption>
</p>

<center>
<p>
In this rendering, you can see how blending the texture into an already existing color affects the shape. Also bilinear
mapping has been used for this image.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/sphere_texture_blend_bilinear.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/6/sphere_texture_replace_bilinear.png" alt="Bilinear Diffuse Texture"/>
  <figcaption>Bilinear Diffuse Texture</figcaption>
</p>

<center>
<p>
The diffuse color of the shape is obtained from the the texture itself in this blending technique.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/sphere_texture_replace_bilinear.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/6/sphere_texture_replace_nearest.png" alt="Nearest Neightbor Mapping"/>
  <figcaption>Nearest Neightbor Mapping</figcaption>
</p>

<center>
<p>
This is the last image of this series :) This one has been added to show the slight difference when we applied the
nearest neighbor mapping while applying the texture.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/sphere_texture_replace_nearest.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/6/skybox.png" alt="Sky Box"/>
  <figcaption>Sky Box</figcaption>
</p>

<center>
<p>
This render is again the basics of texture mapping : Sphere and mesh textures.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/skybox.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/6/killeroo_diffuse_specular_texture.png" alt="Killeroo"/>
  <figcaption>Killeroo</figcaption>
</p>

<center>
<p>
This image is the Killeroo again, but with a bit more fancy walls :) The shapes in the walls are obtained by
mapping a similar looking image onto them. The rest is the same old killeroo.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/killeroo_diffuse_specular_texture.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/6/perlin_types.png" alt="Perlin Types"/>
  <figcaption>Perlin Types</figcaption>
</p>

<center>
<p>
This image contains only Perlin noise types. Also directional light has been used in this particular scene, and
the shadows are problematic because of a bug in this lighting type. I will upload an updated version of this scene once
I handled this bug.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/6/perlin_types.xml">here</a>.
</p>
</center>


<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
