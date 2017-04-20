---
title: "Ray Tracer Vol4"
layout: post
date: 2017-04-10 11.00
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
<center> Step 4 </center>
<center>
<p>
This is the fourth step of my Ray Tracer homework. In this homework, I have implemented two of the most 
essential visual effects : Reflection, and Refraction. In other words, mirrors and transparency.
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p align="center">
  <img src="../assets/images/cornellbox_glass.png" alt="CornellBox"/>
  <figcaption>CornellBox</figcaption>
</p>
<center>

<p>
This is the output of Cornellbox, which is a scene in which both reflection and refraction can be seen. With
the implementation of these two effects, the execution time of my ray tracer has again increased, but I think 
there is still room for improvement. This 800x800 image took around 3.7 seconds.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/cornellbox_glass.xml">here</a>.
</p>
</center>

<p align="center">
  <img src="../assets/images/killeroo_glass.png" alt="Glass Killeroo"/>
  <figcaption>Glass Killeroo</figcaption>
</p>

<center>
<p>
This image is the output of Glass Killeroo, whose resolution is again 800x800. Unlike mirrors, the execution of 
transparency takes really long. In this case, it is 38 seconds.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/killeroo_glass.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/killeroo_half_mirror.png" alt="Half Mirror Killeroo"/>
  <figcaption>Half Mirror Killeroo</figcaption>
</p>

<center>
<p>
This image is the output of Killeroo, another 800x800 image. It takes 6.5 seconds to render the scene.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/killeroo_half_mirror.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/killeroo_mirror.png" alt="Mirror Killeroo"/>
  <figcaption>Mirror Killeroo</figcaption>
</p>

<center>
<p>
This image is the last output of Killeroo's, the mirror killeroo, whose resolution is again 800x800. 8 seconds
is more than enough to get this output.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/killeroo_mirror.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/glass_plates.png" alt="Glass Plates"/>
  <figcaption>Glass Plates</figcaption>
</p>

<center>
<p>
This scene includes only the transparency, but I think it shows its effects really well. This scene took around
6.5 seconds.

The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/glass_plates.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/horse_and_glass_mug.png" alt="Horse and Glass Mug"/>
  <figcaption>Horse and Glass Mug</figcaption>
</p>

<center>
<p>
And now, last but not the least, you can see the famous horse and mugs scene, with a difference: glass mug. 
This scene takes around a minute to render.


The link to the input file is 
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/4/horse_and_glass_mug.xml">here</a>.
</p>
</center>


<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
