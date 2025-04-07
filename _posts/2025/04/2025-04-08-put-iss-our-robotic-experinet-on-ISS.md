---
layout: single
title: "PUT-ISS: Our robotics experiment on the ISS"
author: [kraft-marek, ptak-bartosz, pieczynski-dominik, aszkowski-przemyslaw, piechocki-mateusz]
modified: 2025-04-08
tags: [space robotics, ISS, computer vision, stereovision, ROS, SLAM]
category: [project]
teaser: "/assets/images/posts/2025/04/put-iss-thumb.webp"
---

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-header.webp" height="300px" />
</p>

We are thrilled to announce that our project, **PUT-ISS**! 

As part of the LeopardISS project, we are set to launch our robotic experiment on the International Space Station (ISS) in collaboration with KP Labs.

The [LeopardISS project](https://www.kplabs.space/projects-and-missions/leopardiss---ignis-mission), developed by KP Labs, is set to launch with the IGNIS mission, in which Polish astronaut Sławosz Uznański-Wiśniewski will participate. It aims to validate AI algorithms in orbit and will feature presentations on cutting-edge space research and Poland’s growing role in the industry.

## Our mission and contribution

Our project aims to develop algorithms for stereo vision and 3D mapping in a real-space environment. It is tailored for planetary rover missions and focuses primarily on lunar-like environments, enabling the rover to autonomously move in the future. Our contribution is not only limited to algorithm development but also includes their optimisation and deployment on the hardware delivered by our partner.

The system is intended to advance the space robotics field and validate the potential of computer vision and autonomous applications for future planetary exploration. Additionally, it demonstrates the ability to deploy a Robotic Operating System on resource limited, ready-to-fly space hardware.

## Computation resources

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-leopard.webp" height="300px" />
</p>

> LeopardISS will be hosted in the ICE Cubes Facility, operated by the ICE Cubes Service, within the ISS Columbus module, enabling real-time communication. This ensures the KP Labs team can monitor and manage operations seamlessly from Earth.

An integral part of our algorithms is their deployment on the LeopardISS platform. The platform is a cutting-edge Data Processing Unit (DPU) with energy-efficient processing cores. However, despite its high-performance processing capabilities, dedicated algorithms optimisation is required to to handle space hardware. Considering the platform possibilities and limitations, the PUT-ISS ecosystem has been developed to ensure full operation and safety requirements.

## Visual data

Robotic planet exploration is in a very early stage. This involves data limitations or even a complete lack of robotic data that meets modern robotic requirements. Therefore, to validate our algorithms, we utilised datasets that imitate the Moon's environment visually. One of them was collected in the Sahara Desert in Morocco, providing real-world imagery. Two other datasets were designed and generated using game engines, providing a wide range of synthetic recordings.

* An example image from Morocco dataset:

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-morocco.webp" height="300px" />
</p>

* An example frame generated in the LunarSim environemnt:

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-lunarsim.webp" height="300px" />
</p>

* An example frame rendered with the IsaacSim simulator:

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-isaacsim.webp" height="300px" />
</p>


## Processing

As mentioned before, our system aims to generate a 3D environment map of the robot's surroundings. The map not only allows for improved robot teleoperation but also enables autonomous rover movement to the base while the communication fails. Based on stereovision cameras, the system builds a three-dimensional map, allowing terrain elevation estimation and obstacle avoidance. The whole development pipeline has a node-based structure established on a Robot Operating System (ROS). Its elements are explained below.

### Trajectory estimation

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-traj.webp" height="300px" />
</p>

The first step of the pipeline is an algorithm that generates the robot trajectory. Based on visual odometry, it generates rover movement between frames, estimating the actual rover position. Accurate and fast movement estimation plays a key role in advanced map estimation. The plots above present example trajectories - the grey ground truth and error-based colour estimation.

### Point cloud generation

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-pc.webp" height="300px" />
</p>

Along with trajectory estimation, the point cloud generation algorithm operates. It uses a pair of synchronised images to calculate the disparity, which represents the feature position difference between the two images. By triangulating the position of these matching pixels and considering the baseline (the distance between the two cameras), the algorithm reconstructs the 3D coordinates of the observed scene, generating a 3D map of local image features. An example point cloud is placed above.

### Terrain 3D mapping

In this step, an algorithm combines the estimated position and local point cloud to generate a global environment map. The OctoMap occupancy grid mapping approach is employed, fulfilling the limitations of computation and memory. The algorithm works iterative, operating on recent data provided by previous nodes. An example map building is presented in the video below: 

<iframe width="1280" height="720" src="https://www.youtube.com/embed/gXqfRrS34hw" title="PUT-ISS | Stereo perception and OctoMap building" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Final results and statistics analysis

<p align="center">
    <img src="/assets/images/posts/2025/04/put-iss-map.webp" height="300px" />
</p>

The image above presents a final output map for one of the prepared datasets. Three experiments were prepared in total, enabling evaluation in different lunar-like environments. In the final step of each experiment, the physical analysis is performed to validate the operation in a real-space environment. 

### The LeopardISS mission along with our PUT-ISS robotic software heads to the ISS in Spring 2025! We are proud to be part of this mission and look forward to the exciting developments ahead. Stay tuned for more updates!
