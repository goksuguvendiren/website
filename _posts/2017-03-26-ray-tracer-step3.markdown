---
title: "Ray Tracer Vol3"
layout: post
date: 2017-03-26 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the third step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 3 </center>
<center>
<p>
This is the third part of my Ray Tracer homework where I have implemented maybe the most essential part of
my Ray Tracer : Bounding Volume Hierarchy.
</p>

<p>
Up to now, for every pixel, I was checking all of the triangles for a hit. Obviously, it was unnecessary 
work for most of the pixels in my previous inputs. Bounding volume hierarchy avoids this and gives 
really impressive results. To make a comparison, it used to take 500 seconds ( :O ) to run horse,
however right now, it only takes 1.3 seconds.

Also, this version contains only BVH for the time being, multi-threading will be implemented for the 
following versions
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

<p align="center">
  <img src="../assets/images/horse.png" alt="Horse as mentioned above."/>
  <figcaption>Horse as mentioned above.</figcaption>
</p>


</center>

<p align="center">
  <img src="../assets/images/dragon.png" alt="Dragon"/>
  <figcaption>Dragon</figcaption>
</p>
<center>

<p>
This is the output of Dragon, whose resolution is 800x800 pixels. The construction of the scene takes 
5.8 seconds on average, and rendering takes 1.1sec.
 
The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw3_inputs/dragon.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/killeroo.png" alt="Killeroo"/>
  <figcaption>Killeroo</figcaption>
</p>

<center>
<p>
This image is the output of Killeroo, whose resolution is again 800x800. Unlike the dragon, the construction
of this scene is rather fast, it takes around 0.6sec, and rendering takes 0.45sec on average.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/hw3_inputs/killeroo.xml">here</a>.
</p>
</center>


<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
