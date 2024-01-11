---
layout: single
title: "A fast, lightweight deep learning vision pipeline for autonomous UAV landing support with added robustness"
author: [pieczynski-dominik, ptak-bartosz, kraft-marek, piechocki-mateusz, aszkowski-przemyslaw]
modified: 2024-01-11
tags: [uav, robotics, computer vision, deep learning]
category: [publication]
teaser: "/assets/images/posts/2024/01/vital-thumb.webp"
---
<BR>

<p align="center">
    <img src="/assets/images/posts/2024/01/vital.webp" height="300px" />
</p>


## Abstract:

Despite massive development in aerial robotics, precise and autonomous landing in various conditions is still challenging. This process is affected by many factors, such as terrain shape, weather conditions, and the presence of obstacles. This paper describes a deep learning-accelerated image processing pipeline for accurate detection and relative pose estimation of the UAV with respect to the landing pad. Moreover, the system provides increased safety and robustness by implementing human presence detection and error estimation for both landing target detection and pose computation. Human presence and landing pad location are performed by estimating the presence probability via segmentation. This is followed by the landing pad keypoints’ location regression algorithm, which, in addition to coordinates, provides the uncertainty of presence for each defined landing pad landmark. To perform the aforementioned tasks, a set of lightweight neural network models was selected and evaluated. The resulting measurements of the system’s performance and accuracy are presented for each component individually and for the whole processing pipeline. The measurements are performed using onboard embedded UAV hardware and confirm that the method can provide accurate, low-latency feedback information for safe landing support.

You can find more about this research in our paper in Engineering Applications of Artificial Intelligence journal: [https://www.sciencedirect.com/science/article/pii/S0952197624000228](https://www.sciencedirect.com/science/article/pii/S0952197624000228)
