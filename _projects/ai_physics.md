---
layout: project
title: AI and Physics
description: AI and Physics in BEE
category: AI and Physics
image: "/assets/images/ai_pathfollow.gif"
icon: 🤖
color: color-purple
tags:
  - BEE
  - C++
  - november 2024
github: https://github.com/yourusername/ai-dashboard
live: https://ai-dashboard-demo.com
featured: true
---

## Overview

For this project I worked in BEE, an engine provided by teachers. It uses an ECS, and this was my first time working with one. In the project, I constructed an A* pathfinding algorithm. But in order for it to work, I start by triangulating a map so that I can make a graph for the agents. On this graph, I can run the A* algorithm.

<div class="image-grid grid-2">
  <figure class="image-figure">
    <img src="/assets/images/ai_triangulation.png" alt="Triangulation">
    <figcaption class="image-caption">Triangulation</figcaption>
  </figure>
  <figure class="image-figure">
    <img src="/assets/images/ai_path_following.gif" alt="A*">
    <figcaption class="image-caption">A* in action</figcaption>
  </figure>
</div>

<br>

After that I worked on the physics, since our agents are still clipping through the wall. The physics work well with the pathfinding, but is not limited to it.

<div class="collage collage-c">
    <img src="/assets/images/ai_astar.gif" alt="Forward kinematics">
    <img src="/assets/images/ai_pathfollow.gif" alt="IK arm">
    <img src="/assets/images/ai_physics-showcase.gif" alt="Walking animation">
</div>