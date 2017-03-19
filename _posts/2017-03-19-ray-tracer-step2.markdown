---
title: "Ray Tracer Vol2"
layout: post
date: 2017-03-10 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the second step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 2 </center>
<center>
<p>
This is the second part of my Ray Tracer homework.
</p>

<p>
In this step, I have implemented instancing, triangle, sphere, and mesh transformations as well as
 smooth rendering. I am running my code on a machine with Intel i5 CPU.
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>


<p align="center">
  <img src="../assets/images/bunny_smooth.png" alt="Bunny Smooth"/>
  <figcaption>Bunny Smooth</figcaption>
</p>
<center>

<p>
This is the output of averaging the normals of the triangles on the mesh. This procedure with this input 
takes approximately 33 seconds. The resolution is 512x512 pixels.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw2_inputs/bunny_smooth.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/horse.png" alt="Horse"/>
  <figcaption>Horse</figcaption>
</p>

<center>
<p>
In this input, we hope the see the result of mesh (and triangle) transformations. The image contains 1500x700
pixels, and takes around 500 seconds to complete.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw2_inputs/horse.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/horse_instanced_highres.png" alt="Instanced Horses"/>
  <figcaption>Instanced Horses</figcaption>
</p>

<center>
<p>
In this case, it is possible to observe the results of transformations, as well as instancing on a complex
mesh. Because of the number of pixels and vertices (and lack of any acceleration structure), the execution 
time has increased dramatically to almost 1500 seconds.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw2_inputs/horse_instanced.xml">here</a>.
</p>

</center>

<p align="center">
  <img src="../assets/images/spheres_transform.png" alt="Transformed Spheres"/>
  <figcaption>Transformed Spheres</figcaption>
</p>
<p>
This last input is for testing sphere transformations. As it can be seen, my program is capable of handling 
such transformations without a problem, with a running time of 0.3 second. 

The link to the input file can be found 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw2_inputs/spheres_transform.xml">here</a>.
</p>

<center>
<p>
</p>

</center>
