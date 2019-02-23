---
title: "Ray Tracer Vol9 : Path Tracer"
layout: post
date: 2017-05-14 11.00
tag: ray tracer
image: ../assets/images/profile.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: This is the ninth step of my homework for the CENG795 - Advanced Ray Tracing course.
jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f320.png" height="20" width="20" align="absmiddle">'
category: project
author: goksuguvendiren
externalLink: false
---
<center> Step 9 : Path Tracer </center>
<center>
<p>
This is the ninth, and last step of my Ray Tracer homework. This week I have added global illumination, and as a result,
things became more realistic, as now, each object contribute to the color of others'.

</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p>
While implementing global illumination, I worked on the Cornell Box scene. First, I rendered it with a point light until
I get a result that is satistying enough. Since last week I did a bit (or lot) of refactoring, my code was working differently
with materials that had BRDFs and the other old ones. Therefore I first made sure global illumination worked, then implemented
the rest.
</p>

<p align="center">
  <img src="../assets/images/9/global_first.png" alt="Global Illumination without Reflection/Refraction"/>
  <figcaption>Global Illumination without Reflection/Refraction</figcaption>
</p>



<p align="center">
  <img src="../assets/images/9/global_second.png" alt="Global Illumination with Reflection/Refraction"/>
  <figcaption>Global Illumination with Reflection/Refraction</figcaption>
</p>


<p>
Now, here global illumination is fully implemented, and a light mesh is used as the light source, and other light sources
are removed. This is the reason why the noise increased all of a sudden. In the following image is rendered using 16 samples
per pixel, but the contribution of objects are pretty visible, especially on the floor and the ceiling. This scene took
around 15 seconds.
</p>

<p align="center">
  <img src="../assets/images/9/global_third.png" alt="Global Illumination"/>
  <figcaption>Global Illumination with 16 samples</figcaption>
</p>

<p>
And here is the result with 128 samples. Noise has decreased significantly, and it is great to see the caustic effect
due to the refractive object. This render took 150 seconds.
</p>

<p align="center">
  <img src="../assets/images/9/global_fourth.png" alt="Global Illumination with 128 samples"/>
    <figcaption>Global Illumination with 128 samples</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/9/cornellbox_ldr.xml">here</a>.
</p>

<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
