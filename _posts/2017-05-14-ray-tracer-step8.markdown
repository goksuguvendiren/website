---
title: "Ray Tracer Vol8"
layout: post
date: 2017-05-14 11.00
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
<center> Step 8 </center>
<center>
<p>
This is the eighth step of my Ray Tracer homework. This week I have added several BRDFs to my ray tracer.

P.S. The blog post is written in 30 May, although the output data is from the time I implemented them :)
</p>

<p>
The input xml files and corresponding running times can still be found below each output image.
</p>

</center>

<p>
The following 6 output contain the inputs for variations of Phong BRDF. They are in the following order :

* Original Phong BRDF
* Modified Phong BRDF
* Modified Normalized Phong BRDF
* Original Blinn-Phong BRDF
* Modified Blinn-Phong BRDF
* Original Normalized Blinn-Phong BRDF

These outputs are obtained around 100ms for each.

</p>

<p align="center">
  <img src="../assets/images/8/brdf_phong_original.png" alt="Original Phong BRDF"/>
  <figcaption>Original Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_phong_original.xml">here</a>.
</p>
</center>



<p align="center">
  <img src="../assets/images/8/brdf_phong_modified.png" alt="Modified Phong BRDF"/>
  <figcaption>Modified Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_phong_modified.xml">here</a>.
</p>
</center>


<p align="center">
  <img src="../assets/images/8/brdf_phong_modified_normalized.png" alt="Modified Normalized Phong BRDF"/>
  <figcaption>Modified Normalized Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_phong_modified_normalized.xml">here</a>.
</p>
</center>



<p align="center">
  <img src="../assets/images/8/brdf_blinnphong_original.png" alt="Original Blinn-Phong BRDF"/>
  <figcaption>Original Blinn-Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_blinnphong_original.xml">here</a>.
</p>
</center>



<p align="center">
  <img src="../assets/images/8/brdf_blinnphong_modified.png" alt="Modified Blinn-Phong BRDF"/>
  <figcaption>Modified Blinn-Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_blinnphong_modified.xml">here</a>.
</p>
</center>



<p align="center">
  <img src="../assets/images/8/brdf_blinnphong_modified_normalized.png" alt="Modified Normalized Blinn-Phong BRDF"/>
  <figcaption>Modified Normalized Blinn-Phong BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_blinnphong_modified_normalized.xml">here</a>.
</p>
</center>



<p>
The following results are the Torrance-Sparrow BRDF. Although I think I implemented it correctly, there is a bug I could
not resolve, therefore these results unfortunately do not appear as they are supposed to do. I will update this post and these outputs
as soon as I solve this issue.
</p>


<p align="center">
  <img src="../assets/images/8/brdf_torrancesparrow.png" alt="Torrance-Sparrow BRDF"/>
  <figcaption>Torrance-Sparrow BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_torrancesparrow.xml">here</a>.
</p>
</center>



<p>
And the killeroo with this Torrance-Sparrow BRDF looks like this :
</p>


<p align="center">
  <img src="../assets/images/8/killeroo_torrancesparrow.png" alt="Torrance-Sparrow BRDF"/>
  <figcaption>Torrance-Sparrow BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_torrancesparrow.xml">here</a>.
</p>
</center>

<p>
Lastly, killeroo with modified normalized Blinn-Phong is like this :
</p>

<p align="center">
  <img src="../assets/images/8/killeroo_blinnphong.png" alt="Torrance-Sparrow BRDF"/>
  <figcaption>Torrance-Sparrow BRDF</figcaption>
</p>
<center>

<p>
The link to the input file is
<a href="https://github.com/goksuguvendiren/AdvancedRayTracing/blob/master/inputs/8/brdf_torrancesparrow.xml">here</a>.
</p>
</center>

<center>
<p>
The github link to my repository is <a href="https://github.com/goksuguvendiren/AdvancedRayTracing">here</a>.
</p>

</center>
