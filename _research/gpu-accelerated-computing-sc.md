---
title: 图形处理器（GPU）加速计算
anchor_id: gpu-accelerated-computing
image: images/speedup.gif
image_url: publications_sc.html#li2020gmd
language: sc
order: 6
---

最新的高性能计算机已经开始广泛使用通用图形处理器（GPU）进行加速计算。作为我在[洛斯阿拉莫斯国家实验室](https://www.lanl.gov){:target="_blank"}的科研项目的一部分，我把一个用于大气海洋边界层湍流模拟的大涡模式（[PALM](https://palm.muk.uni-hannover.de/trac){:target="_blank"}）移植到GPU上做加速计算。在这项工作中，我利用一个基于指令的性能可移植的并行计算编程模型[OpenACC](https://www.openacc.org){:target="_blank"}和NVIDIA CUDA快速傅里叶变换软件包[cuFFT](https://developer.nvidia.com/cufft){:target="_blank"}，将PALM的一个定制版本移植到了GPU。初步结果显示，相比于单个CPU，单个GPU可以实现总体上超过10倍的计算加速。如旁边的这幅图所示，目前的计算加速主要受限于快速傅里叶变换的效率。不过，通过进一步提高循环效率和优化数据局部性，有望可以实现更大的计算加速。GPU加速计算技术为数值模拟研究海洋边界层湍流混合过程提供了更有效的工具。详情请参见发表论文[[12]](publications_sc.html#li2020gmd")。
