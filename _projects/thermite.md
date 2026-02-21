---
layout: project
title: Raytracing
description: Raytracing in a Template project
category: Rendering
image: "/assets/images/ray_glass.png"
icon: 🤖
color: color-purple
tags:
  - Template
  - C++
  - april 2024
github: https://github.com/yourusername/ai-dashboard
live: https://ai-dashboard-demo.com
featured: true
---

## Overview

In this project I worked on a template that had the bare basics of a ray tracer. Going into this, I hadn't worked with a raytracer before, apart from raytracing in one weekend for preparation for the project. I started with simple features like point lights and directional light and eventually I worked my way towards more impressive features.

<div class="image-grid grid-2">
  <figure class="image-figure">
    <img src="/assets/images/ray_areal.png" alt="Area light">
    <figcaption class="image-caption">Area Light</figcaption>
  </figure>
  <figure class="image-figure">
    <img src="/assets/images/ray_refglos.png" alt="Glossy reflections">
    <figcaption class="image-caption">Glossy Reflections</figcaption>
  </figure>
</div>

<br>

I also worked on reprojection, the difference is dramatic — noisy without it, clean with it:

<div class="image-grid grid-2">
  <figure class="image-figure">
    <img src="/assets/images/ray_norepr.png" alt="Without reprojection">
    <figcaption class="image-caption">Without Reprojection</figcaption>
  </figure>
  <figure class="image-figure">
    <img src="/assets/images/ray_repr.png" alt="With reprojection">
    <figcaption class="image-caption">With Reprojection</figcaption>
  </figure>
</div>

<br>

And finally, the most impressive feature I worked on during the block was glass. The glass sphere below features snell's law for refraction and fresnel equations for reflection. The reflection is most noticable around the edges of the sphere in the image.

<figure class="image-figure">
  <img src="/assets/images/ray_glass.png" alt="Glass sphere">
  <figcaption class="image-caption">Glass with refraction and reflection</figcaption>
</figure>