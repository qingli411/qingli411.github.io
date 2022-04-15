---
title: GPU accelerated computing
anchor_id: gpu-accelerated-computing
image: /images/speedup.gif
image_url: publications.html#li2020gmd
language: en
order: 6
---

General-purpose graphics processing units (GPUs) have rapidly evolved to become high performance accelerators for modern supercomputers. I have been working on accelerating the large eddy simulations (LES) using GPUs. I have ported a customized version of [PALM](https://palm.muk.uni-hannover.de/trac){:target="_blank"} on GPU using [OpenACC](https://www.openacc.org){:target="_blank"}, a directive-based and performance-portable parallel programming model, and [cuFFT](https://developer.nvidia.com/cufft){:target="_blank"}, the NVIDIA CUDA Fast Fourier Transform library. Preliminary results with a single GPU show more than 10 times overall speedup versus using a single CPU, limited primarily by the relatively slow parallel Fast Fourier Transform algorithm, though additional speedup is still possible by further optimizing the loops and data locality. See more in paper [[12]](publications.html#li2020gmd").
