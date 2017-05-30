---
title: "Ray Tracer Vol7"
layout: post
date: 2017-04-30 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the seventh step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 7 </center>
<center>
<p>
This is the seventh step of my Ray Tracer homework. This week I have added bump mapping functionality to my ray tracer.

P.S. The blog post is written in 30 May, although the output data is from the time I implemented them :)
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p align="center">
  <img src="../assets/images/7/bump_mapping_basic.png" alt="Simple Bump Mapping"/>
  <figcaption>Simple Bump Mapping</figcaption>
</p>
<center>

<p>
This image shows the main functionality of bump mapping. Normals are updated according to the gradients of the texture, and
therefore the image looks more detailed than it actually is. This image took 21 seconds to render.

In this week's implementation, I find that my bump maps are rather more dominant, though they don't seem wrong to me.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/7/bump_mapping_basic.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/7/bump_mapping_transformed.png" alt="Transformation of Bump Mapping"/>
  <figcaption>Transformation of Bump Mapping</figcaption>
</p>

<center>
<p>
With this output, you can see that bump mapping works well with transformations. This output also took 27 seconds.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/7/bump_mapping_transformed.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/7/killeroo_bump_walls.png" alt="Killeroo"/>
  <figcaption>Killeroo</figcaption>
</p>

<center>
<p>
This is the Killeroo with detailed walls :) Took 28 seconds.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/7/killeroo_bump_walls.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/7/sphere_bump_nobump.png" alt="World No Bump - Bump"/>
  <figcaption>World No Bump - Bump</figcaption>
</p>

<center>
<p>
This is the last image where you can see and compare the results of bump mapping with the world texture. While the one
on the left looks too artificial, bump mapped version looks more realistic. This image took 13 seconds.
</p>
<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/7/sphere_bump_nobump.xml">here</a>.
</p>
</center>

<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
