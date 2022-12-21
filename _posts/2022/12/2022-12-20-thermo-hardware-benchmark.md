---
layout: single
title: "Efficient People Counting in Thermal Images: The Benchmark of Resource-Constrained Hardware"
author: [piechocki-mateusz, kraft-marek, aszkowski-przemyslaw, pieczynski-dominik]
modified: 2022-12-20
tags: [thermal, unet, hardware, benchmark]
category: [publication]
teaser: "/assets/images/posts/2022/12/single_gaussian.webp"
---

<p align="center">
    <img src="/assets/images/posts/2022/12/thermo-hardware-benchmark-graphical-abstract.webp" height="300px" />
</p>

## Abstract:

> The monitoring of presence is a timely topic in intelligent building management systems. Nowadays, most rooms, halls, and auditoriums use a simple binary presence detector that is used to control the operation of HVAC systems. This strategy is not optimal and leads to significant amounts of energy being wasted due to inadequate control of the system. Therefore, knowing the exact person count facilitates better adjustment to current needs and cost reduction. The vision-based people-counting is a well-known area of computer vision research. In addition, with rapid development in the artificial intelligence and IoT sectors, power-limited and resource-constrained devices like single-board computers or microcontrollers are able to run even such sophisticated algorithms as neural networks. This capability not only ensures the tiny size and power effectiveness of the device but also, by definition, preserves privacy by limiting or completely eliminating the transfer of data to the cloud. In this paper, we describe the method for efficient occupancy estimation based on low-resolution thermal images. This approach uses a U-Net-like convolutional neural network that is capable of estimating the number of people in the sensor’s field of view. Although the architecture was optimized and quantized to fit the limited microcontroller’s memory, the metrics obtained by the algorithm outperform the other state-of-the-art solutions. Additionally, the algorithm was deployed on a range of embedded devices to perform a set of benchmarks. The tests carried out on embedded processors allowed the comparison of a wide range of chips and proved that people counting can be efficiently executed on resource-limited hardware while maintaining low power consumption.

You can find more about this project in [this publication](https://ieeexplore.ieee.org/document/9964383) or in [its repository](https://github.com/PUTvision/thermo-hardware-benchmark).

### Achieved Results

<p align="center">
    <img src="/assets/images/posts/2022/12/achieved_results.webp" height="130px" />
</p>

#### Hardware Performance

<p align="center">
    <img src="/assets/images/posts/2022/12/hardware_performance.webp" height="650px" />
</p>
