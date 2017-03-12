---
title: "Ray Tracer"
layout: post
date: 2017-03-10 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 1 </center>
<center>
<p>
This is the first homework of my Ray Tracer for the course Ceng795 - Advanced Ray Tracer. Below, the images 
have been resized to 512x512, after they had been rendered with full resolution.
</p>

<p>
Up to now, I have implemented the very basics of a ray tracer : Ambient, Diffuse, Phong reflectance, 
and shadows. Currently there is not any acceleration step, so the execution times are not very impressive.
</p>

<p>
All the input xml files for which these outputs have been produced are given below each image, and execution
times are calculated by running the program 10 times and taking its average.
</p>

</center>


<p align="center">
  <img src="../assets/images/simple.png" alt="Simple" height="512" width="512"/>
  <figcaption>Simple</figcaption>
</p>

<center>
<p>
This is the most basic input of all. Tests for sphere and triangle intersections, and 
800x800 resolution takes 0.14 seconds on average to complete.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/simple.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/simple_shading.png" alt="Simple Shading" height="512" width="512"/>
  <figcaption>Simple Shading</figcaption>
</p>

<center>
<p>
In this case, the effects of light sources are more comprehensible, by the Phong highlight and shadow of the 
sphere. 800x800 resolution takes 15.7 seconds on average.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/simple_shading.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/bunny.png" alt="Bunny" height="512" width="512"/>
  <figcaption>Bunny</figcaption>
</p>

<center>
<p>
This is the output of a complex mesh, and probably the most satisfactory one, although it may take a little 
longer to see the results :) All the effects of lights are again visible in this image, and it takes around 
... seconds to run.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/bunny.xml">here</a>.

</center>

<p align="center">
  <img src="../assets/images/bunny_normals.png" alt="Bunny Normals" height="512" width="512"/>
  <figcaption>Bunny Normals</figcaption>
</p>


<center>
<p>
Also, although it is not result of a light effect or complex material, I think it looks really nice when the
surface normals of the triangles are printed instead of colors, so I wanted to include it as a promotion :)
</p>

</center>
