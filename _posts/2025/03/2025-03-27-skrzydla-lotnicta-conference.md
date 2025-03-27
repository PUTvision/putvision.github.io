---
layout: single
title: "Conference Skrzydła Lotnictwa with Best Poster Award"
author: [zacholski-piotr, pieczynski-dominik, kraft-marek]
modified: 2025-03-25
tags: [computer vision, deep learning, uav, metric learning]
category: [conference]
teaser: "/assets/images/posts/2025/03/sl_conference_teaser.webp"
---

<p align="center">
    <img src="/assets/images/posts/2025/03/sl_conference.webp" height="300px" />
</p>

"Skrzydła Lotnictwa 2025" conference, organized by the "Koło Naukowe Bezpieczeństwo i Zarządzanie Lotnictwem", was held at the Lecture Center of Poznan University of Technology on March 25. The event brought together experts, students and representatives of the aviation industry from all over Poland, focusing on three main thematic blocks: safety in civil aviation, sustainable development and aviation infrastructure and operations.

## Poster session
As part of the poster session, our team was represented by Piotr Zacholski, who presented a paper entitled. “Prosta is skuteczna metoda nawigacji bez GPS, nawigacja dronem przy użyciu systemów wizyjnych”, prepared by Piotr Zacholski, Dominik Pieczyński and Mark Kraft. The project demonstrates that vision-based navigation systems can provide an independent alternative to the GPS signal - especially where its availability is limited or prone to interference. By analyzing images from the onboard compass camera, the drone can autonomously orient itself in space on a known map. We are proud to announce that our poster was awarded the prize for the best conference poster. This is a great motivation for us to further develop this line of research and technology.

## Poster abstract
> UAV localization without the use of GPS is a significant challenge in the navigation of autonomous systems in the face of the possibility of signal interference. The presented algorithm solves this problem based on image analysis. The main difficulty in this task is to efficiently searching a large space and minimizing the localization error with limited resources computational resources. Standard approaches based on random sampling are very time-consuming, which limits its effectiveness in practical applications. This paper compares two UAV localization strategies based on matching local binary patterns (LBP) and a particle filter: (1) a method in which samples are generated randomly and then processed by a particle filter, and (2) an approach using a network of metrically learned neural network that, prior to sample generation, identifies areas with high probability of correct location, reducing the search space and speeding up convergence due to better initialization. The neural network model was trained on a set of National Agriculture Imagery Program (NAIP) data, which provides high-resolution aerial images, enabling realistic simulation of visual navigation conditions and matching the model to the characteristics of the analyzed images. Experimental results show that the use of pre-selection of areas leads to a faster and more stable localization process compared to a fully random approach. The reduction in search space results in fewer iterations needed for correct position estimation and a reduction in UAV localization error. The results obtained indicate that the combination of particle filter, LBP matching and region selection by a neural network represents an effective method for visual navigation without GPS, offering greater precision and a significant reduction in processing time.

Thank you to the organizers and all participants for the inspiring atmosphere. We are already looking forward to the next edition!