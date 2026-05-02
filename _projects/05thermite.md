---
layout: project
title: Thermite
team: 16
description: AI Programming in a Custom Engine
category: AI
image: "/assets/images/tmt_navmesh.png"
icon: 🤖
color: color-purple
tags:
  - Thermite Engine
  - C++
  - november 2025
github: https://github.com/yourusername/ai-dashboard
live: https://ai-dashboard-demo.com
featured: true
---

## Overview

In this custom engine project I worked mainly on navigation for AI. The game is set in space, and the enemies are supposed to walk on the asteroids that are floating around. In order for the enemies to do that, I made a navmesh system that could make a navmesh from voxel data (64trees). There were a few issues with the initial concept. First of all, generation took very long, and caused major lagspikes. To fix this, I do the navmesh generation over time. And, if I'm doing the generation over time anyway, I might aswell first go one level higher in the 64tree to quickly generate a lower level of detail mesh wich the enemy can immediately start using while a higher level of detail mesh is being made.

Also, because on asteroids there isn't really an 'up', I had to come up with a way to know where the ground was, so that the enemy always faces the ground. The most straight forward way to know what 'up' is, is by looking at the ground normal. There wasn't an easy way to compute the normals, because the connections some nodes had created caused a few cases where a simple crossproduct would be inaccurate. To fix these edge cases, I simply average all the normals by comparing them to their neighbours. This was also quite slow, so I also do it over time. All these things together make for quite a nice visualisation, wich can be seen below:

<video src="/assets/images/tmt_nm_gen.mp4" autoplay loop muted playsinline></video>
<figcaption class="image-caption">navmesh generation over time</figcaption>

And then we can have a procedural walker traverse the navmesh:

<video src="/assets/images/tmt_walk.mp4" autoplay loop muted playsinline></video>
<figcaption class="image-caption">prototype of procedural walker on navmesh</figcaption>