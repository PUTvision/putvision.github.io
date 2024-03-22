---
layout: single
title: "ISO-compatible personal temperature measurement using visual and thermal images with facial region of interest detection"
author: [ptak-bartosz, aszkowski-przemyslaw, kraft-marek]
modified: 2023-11-21
tags: [computer vision, RGB-D, thermal camera, temperature measurement, facial region of interest detection]
category: [publication]
teaser: "/assets/images/posts/2024/03/face-thumb.webp"
---
<BR>

<p align="center">
    <img src="/assets/images/posts/2024/03/face-abstract.webp" height="300px" />
</p>


## Abstract:

Disease outbreaks and pandemics show us how important it is to limit the spread of diseases. One common indicator of many ailments is body temperature. It’s a measurement that can be taken quickly, also using contactless methods. However, it is necessary to ensure the methodological correctness, repeatability and reliability of such measurement. In this manuscript, we introduce a non-intrusive approach for individual body temperature assessment that adheres to the stipulated criteria outlined by ISO/IEC 80601-2-59 standard. The measurements are performed at specific regions of interest (ROIs) of a human face, at the inner canthi of both eyes, which show high robustness to the environment temperature change. The method utilises the fusion of RGB-D (red, green, blue and depth) and thermal cameras. The system detects the ROIs on the RGB image employing deep learning methods and transfers them to the thermal image, from which the temperature can be read. The system was tested on our validation dataset consisting of 210 individuals, achieving ROI’s position identification mean error below 3 mm and temperature measurement error below 0.5°C, which is in line with the ISO norm requirements.

You can find more about this research in our paper in IEEE Access journal: [https://ieeexplore.ieee.org/document/10472492](https://ieeexplore.ieee.org/document/10472492)
