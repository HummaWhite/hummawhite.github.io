---
layout: page
title: Projects
background: '/img/teapot3.png'
---

The projects listed below could have had their own development blogs, but time is quite limited... Perhaps I'll write some when I'm free.

---
## SVGF
I replicated SVGF from [this paper](https://research.nvidia.com/publication/2017-07_Spatiotemporal-Variance-Guided-Filtering%3A) in November 2021. [The result page](SVGF/).

Still, the performance of my implementation demands to be improved, since the 5-level A-trous wavelet runs about 50ms on my 1050ti. So code will come later when I'm free to do so.

---
## Zillum Renderer

<center>
	<img src="/img/ui.png" width="100%" />
</center>

[Zillum](https://github.com/HummaWhite/Zillum) is my renderer, under development since I seriously began to study realistic image synthesis in Sep 2020. Now it has two versions, one running on CPU, another on GPU by OpenGL compute shader, which is named [ZillumGL](https://github.com/HummaWhite/ZillumGL).
 
I made three videos about the GPU version in 2021, you can view them through the links: [Low-discrepancy sampler test](https://youtu.be/pjfcD8fYfQg), [Rendering the Gallery scene](https://youtu.be/TGbwSyqxKvY), [Rendering the Utah Teapot](https://youtu.be/HNXanaqzhgQ). Also, see pictures in the GALLERY section.

Typically when I learn new rendering algorithms, I'll first try to implement them in Zillum, then I would think how to implement those on GPU and optimize. I've implemented path tracing, adjoint particle tracing and bidirectional path tracing integrators in Zillum. And for ZillumGL, I implemented path tracing and adjoint particle tracing. Both versions now support MTBVH, environment map importance sampling and multiple BSDF models. When it's appropriate, I think I would consider merging the two versions into one software.

---
## Parallel & Distributed Computing Course Lab Project
There were two programming labs in the course this year (2021).
My programs were the best optimized in the class, which earned me 100% score of the lab part : ) (the faster your program, the higher your score).

I cannot share my code, but ideas can be communicated. Presentation slides (in Chinese): [MPI Prime Sieve](Parallel/MPI_prime_sieve.pdf), [CUDA N-Body](Parallel/CUDA_nbody.pdf)

---
## Software Rasterizer
In the month before I started to learned offline rendering, I tried to implement a [software rasterizer](https://github.com/HummaWhite/SoftRaster) which emulates the functions of modern hardware graphics pipelines. It supports programmable vertex shader and fragment shader.
