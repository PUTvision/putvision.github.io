---
layout: single
title: "Estimation of corn crop damage caused by wildlife in UAV images"
author: [aszkowski-przemyslaw, kraft-marek, pieczynski-dominik]
modified: 2024-09-22
tags: [computer vision, agriculture, segmentation, UAV]
category: [publication]
teaser: "/assets/images/posts/2024/09/corn_field_thumb.webp"
---
<BR>

<p align="center">
    <img src="/assets/images/posts/2024/09/corn_fields.webp" height="300px" />
</p>

We are happy to announce our recent publication about estimating corn crop damages from UAVs images!

## Abstract:

This paper proposes a low-cost and low-effort solution for determining the area of corn crops damaged by the wildlife facility utilising field images collected by an unmanned aerial vehicle (UAV). The proposed solution allows for the determination of the percentage of the damaged crops and their location. The method utilises models based on deep convolutional neural networks (e.g., UNet family) and transformers (SegFormer) trained on over 300 hectares of diverse corn fields in western Poland. A range of neural network architectures was tested to select the most accurate final solution. The tests show that despite using only easily accessible RGB data available from inexpensive, consumer-grade UAVs, the method achieves sufficient accuracy to be applied in practical solutions for agriculture-related tasks, as the IoU (Intersection over Union) metric for segmentation of healthy and damaged crop reaches 0.88.

You can find more about this research in our paper in Precision Agriculture journal: [http://dx.doi.org/10.1007/s11119-024-10180-7](http://dx.doi.org/10.1007/s11119-024-10180-7)
