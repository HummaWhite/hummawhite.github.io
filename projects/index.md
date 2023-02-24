---
layout: page
title: Projects
background: '/img/teapot3.png'
---

---
## EIDOLA - Vulkan Real-Time Ray Tracer
CIS 565 final project. We implemented a real-time path tracer with Vulkan, ReSTIR DI [Bitterli et al. 2020], ReSTIR GI [Ouyang et al. 2021] and a denoiser (actually A-Trous). We're able to make it 50 FPS for the Bistro scene.
<div align="center">
	<img src="https://raw.githubusercontent.com/IwakuraRein/CIS-565-Final-VR-Raytracer/restir-direct/images/bistro_ext.jpg" width="100%" />
</div>

[Repo](https://github.com/IwakuraRein/CIS-565-Final-VR-Raytracer) and [demo video](https://youtu.be/cIA90Zalupw)

---
## CUDA Path Tracer
CIS 565 Project 3. Because I had two Zillum renderers before, I'd like to call this project [ZillumCU](https://github.com/HummaWhite/Project3-CUDA-Path-Tracer).

What was different in this project compared to my other two renderers is that I tried to add support for PBR textures. The result turned out to be very stunning. Even I myself was amazed when I saw that camera.

I told Shehzan this project would be a big surprize, and it was. [You can see their evaluation here](www.linkedin.com/feed/update/urn:li:activity:6994496086274883584)

<div align="center">
	<img src="https://raw.githubusercontent.com/HummaWhite/Project3-CUDA-Path-Tracer/main/img/photo_realistic.jpg" width="100%" />
</div>

---
## SVGF
Update in 2022:
One year later, I reimplemented SVGF as the 4th project of CIS 565. This time it's build on CUDA with better code structure, better quality and (probably) better performance. Execept using position difference instead of clip space depth derivatives to drive the filter kernel, this implementation replicates every point mentioned in the paper.

You can find the project repo and my report for the project [here](https://github.com/HummaWhite/Project4-CUDA-Denoiser)

Original post:
I implementted SVGF from [this paper](https://research.nvidia.com/publication/2017-07_Spatiotemporal-Variance-Guided-Filtering%3A) in November 2021. [The result page](SVGF/).

Still, the performance of my implementation demands to be improved, since the 5-level A-trous wavelet runs about 50ms on my 1050ti. So code will come later when I'm free to do so.

---
## Zillum Renderer

<center>
	<img src="/img/ui.png" width="100%" />
</center>

[Zillum](https://github.com/HummaWhite/Zillum) is my renderer, under development since I seriously began to study realistic image synthesis in Sep 2020. Now it has two versions, one running on CPU, another on GPU by OpenGL compute shader, which is named [ZillumGL](https://github.com/HummaWhite/ZillumGL).

I made three videos about the GPU version in 2021, you can view them through the links: [Low-discrepancy sampler test](https://youtu.be/pjfcD8fYfQg), [Rendering the Gallery scene](https://youtu.be/TGbwSyqxKvY), [Rendering the Utah Teapot](https://youtu.be/HNXanaqzhgQ). Also, see pictures in the GALLERY section.

Typically when I learn new rendering algorithms, I'll first try to implement them in Zillum, then I would think how to implement those on GPU and optimize. I've implemented path tracing, adjoint particle tracing and bidirectional path tracing integrators in Zillum. And for ZillumGL, I implemented path tracing and adjoint particle tracing. Both versions now support MTBVH, environment map importance sampling and multiple BSDF models. When it's time, I think I would consider merging the two versions into one.

---
## Parallel & Distributed Computing Course Project
There were two programming labs in the course this year (2021). The first was MPI prime sieve, the second was CUDA N-body problem.
My programs were the best optimized in the class, which earned me 100% of performance grade : ) (the faster your program, the higher your grade).

In the first program I did something crazy: writing intrinsic AVX2 assembly in C++.

If you are interested in the detail of my implementation, you can see my presentation slides (although in Chinese): [MPI Prime Sieve](Parallel/MPI_prime_sieve.pdf), [CUDA N-Body](Parallel/CUDA_nbody.pdf)

<center>
	<img src="/img/avx2.jpg" width="100%" />
</center>

---
## Software Rasterizer
In the month before I started to learned offline rendering, I tried to implement a [software rasterizer](https://github.com/HummaWhite/SoftRaster) which emulates the functions of modern graphics pipeline. You can write programmable vertex shader and fragment shader with it.
