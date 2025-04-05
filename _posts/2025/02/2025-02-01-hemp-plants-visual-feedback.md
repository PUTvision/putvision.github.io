---
layout: single
title: "Visual Feedback System Supporting Robotic Manipulation of Hemp Plants"
author: [kraft-marek, ptak-bartosz, piechocki-mateusz, pieczynski-dominik]
modified: 2025-02-01
tags: [hemp, computer vision, deep learning, robotics, manipulation]
category: [publication]
teaser: "/assets/images/posts/2025/02/hemp-thumb.webp"
---

<p align="center">
    <img src="/assets/images/posts/2025/02/hemp-header.webp" height="300px" />
</p>

## Abstract:

> This paper presents an agricultural robotics system designed to automate the detection and manipulation of male hemp plants, addressing the challenge of manually removing these to enhance crop quality. The solution uses an industry-standard, inexpensive RGB-D camera as the input data source to derive control signals controlling the robotic arm and end effector. Input image data processing is performed by a dedicated neural network model trained using a dataset created specifically for the described task to achieve detection by stalk segmentation and postprocessing. The research involved assessing various neural network models, including UNet, DeepLabV3+, and YOLOv8 in various variants, for their capability to detect stalks accurately and swiftly. Fast operation is necessary for effective real-time feedback in robotic grasping tasks. Among tested architectures, the integration of UNet with ResNet50 was found to provide a good trade-off between detection precision and operational speed on edge AI devices. The resulting solution offers good accuracy and significantly outperforms existing methods in terms of processing speed, promising substantial improvements in agricultural robotics by enabling on-line adaptive grasping using low-cost components. The applications can be extended beyond hemp tending to include various other crops, eliminating tedious manual labor.

Link to the publication: [https://www.tandfonline.com/doi/full/10.1080/15440478.2025.2454261](https://www.tandfonline.com/doi/full/10.1080/15440478.2025.2454261)
