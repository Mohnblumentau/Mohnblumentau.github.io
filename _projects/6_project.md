---
layout: page
title: Disparity Algorithm
description: Correspondence-based pairwise depth estimation with parallel acceleration
img: assets/img/BachelorThesis.PNG
importance: 1
category: bachelor
---

The thesis covers the implementation and evaluation of a stereo vision correspondence-based depth estimation algorithm on a GPU. The results and feedback are used for a Multi-view camera system in combination with Jetson TK1 devices for parallelized image processing and the aim of this system is to estimate the depth of the scenery in front of it. The performance of the algorithm plays the key role. Alongside the implementation, the objective of this study is
to investigate the advantages of parallel acceleration inter alia the differences to the execution on a CPU which are significant for all the function, the imposed overheads particular for a GPU application like memory transfer from the CPU
to the GPU and vice versa as well as the challenges for real-time and concurrent execution. The study has been conducted with the aid of CUDA on three NVIDIA GPUs with different characteristics and with the aid of knowledge
gained through extensive literature study about different depth estimation algorithms but also stereo vision and correspondence as well as CUDA in general. Using the full set of components of the algorithm and expecting (near) real-time
execution is utopic in this setup and implementation, the slowing factors are inter alia the semi-global matching. Investigating alternatives shows that results for disparity maps of a certain accuracy are also achieved by local methods like the Hamming Distance alone and by a filter that refines the results. Furthermore, it is demonstrated that the kernel launch configuration and the usage of GPU memory types like shared memory is crucial for GPU implementations and has an impact on the performance of the algorithm. Just concurrency proves to be a more complicated task, especially in the desired way of realization. For the future work and refinement of the algorithm it is therefore recommended to invest more time into further optimization possibilities in regards of shared memory and into integrating the algorithm into the actual pipeline.

Read my full thesis <a href="http://www.diva-portal.org/smash/record.jsf?pid=diva2%3A1247193&dswid=262">here</a>.