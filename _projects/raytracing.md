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

In this project I worked on a template that had the bare basics of a ray tracer. Going into this, I hadn't worked with a raytracer before, apart from raytracing in one weekend for preperation for the project. I started with simple features like point lights and directional light and eventually I worked my way towards more impressive features. This includes an area light:

![](/assets/images/ray_areal.png)

Glossy reflections:

![](/assets/images/ray_refglos.png)

And reprojection. The top image shows how noisy the image looks without reprojection, and the bottom image is noise-free because of reprojection:

![](/assets/images/ray_norepr.png)
![](/assets/images/ray_repr.png)

And finally, the most impressive feature I worked on during the block was glass. The glass sphere below features snell's law for refraction and fresnel equations for reflection. The reflection is most noticable around the edges of the sphere in the image.

![](/assets/images/ray_glass.png)