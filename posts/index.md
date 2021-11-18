---
layout: page
title: Projects
background: '/img/teapot3.png'
---

The projects listed below could have had their own development blogs, but time is quite limited... Perhaps I'll add some when I'm free.

## Zillum Renderer
[Zillum](https://github.com/HummaWhite/Zillum) is my ray tracer, under development since I seriously began to study realistic image synthesis in Sep 2020. Now it has two versions, one running on CPU, another on GPU by OpenGL compute shader, which is also named [ZillumGL](https://github.com/HummaWhite/ZillumGL).
I've made videos about the GPU version, you can view them through the links: [Low-discrepancy sampler test](https://youtu.be/pjfcD8fYfQg), [Rendering the Gallery scene](https://youtu.be/TGbwSyqxKvY)

Typically when I want to verify new light transport methods I learn, I'll first code them in the CPU version, then I would consider how to implement those on GPU and optimize.

---
## Software Rasterizer
In the month before I started to learned offline rendering, I tried to implement a [software rasterizer](https://github.com/HummaWhite/SoftRaster) which emulates the functions of modern hardware graphics pipelines. It supports programmable vertex shader and fragment shader.

---
## The Final Project of C++ Programming Course
My final project for C++ Programming (fall 2019). We were required to make a sprite game, so I made a very simpified duplicate of A LINK TO THE PAST, Github repo [here](https://github.com/HummaWhite/cpp2019).

---
### 3D Model for the Administrative Building of No.7 High School Chengdu
In 2018 I had thought of making such a model for my high school. For some reasons, it was until Jan 2020 I finally finished it (just before I knew Graphics). I build this model by direct observation of the building, with help from some historical images and lengths I measured at the ground level. Git repo [here](https://github.com/HummaWhite/3DProject).

In 2020 I could only use Blender to render this model, to celebrate the 115th anniversary of my high school. A year later I'm able to render it with my own renderer!
