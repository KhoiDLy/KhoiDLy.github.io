---
title: Electro-Hydraulic Rolling Soft Wheel:  Design, Hybrid Dynamic Modeling, and Model Predictive Control
# link: https://github.com/alecive/periPersonalSpace
# link-alt: GitHub repository
img: RollingRobot_Sequence.jpg
img-thumb: RollingRobot_Sequence_thumb.jpg
alt: Electro-Hydraulic Rolling Soft Wheel:  Design, Hybrid Dynamic Modeling, and Model Predictive Control
description: Electro-hydraulic rolling soft robot
tags: [research,robotics,icub,robot,humanoids,double touch,self touch,inverse kinematics,denavit-hartenberg,dh parameters,ipopt,optimization,cognitive robotics,body representations,icra,icra 2014,body schema,open source,github]
authors: Khoi Ly, Jatin Mayekar, Sarah A. Manzano, Christoph Keplinger, Mark Rentschler, Nikolaus Correll
submission: IEEE Transactions on Robotics, 2022
paper_pdf: "2022_KhoiLy_Electro-Hydraulic_Rolling_Soft_Wheel"
paper_title: "Electro-Hydraulic Rolling Soft Wheel: Design, Hybrid Dynamic Modeling, and Model Predictive Control"
---
## Abstract

Locomotion through rolling is attractive compared to other forms of locomotion thanks to uniform designs, high degree of mobility, dynamic stability, and self-recovery from collision. Despite previous efforts to design rolling soft systems, pneumatic and other soft actuators are often limited in terms of high-speed dynamics, system integration, and/or functionalities. Furthermore, mathematical description of the rolling dynamics for this type of robot and how the models can be used for speed control are often not mentioned. This article introduces a cylindrical-shaped shell-bulging rolling soft wheel that employs an array of 16 folded-HASEL actuators as a mean for improved rolling performance. The actuators represent the soft components with discrete forces that propel the wheel, whereas the wheel's frame is rigid but allows for smooth, continuous change in position and speed. We discuss the interplay between the electrical and mechanical design choices, the modeling of the wheel's hybrid (continuous and discrete) dynamic behavior, and the implementation of a model predictive controller (MPC) for the robot's speed. With the balance of several design factors, we show the wheel's ability to carry integrated hardware with a maximum rolling speed at 0.7 m/s (or 2.2 body lengths per second), despite its total weight of 979 g, allowing the wheel to outperform the existing rolling soft wheels with comparable weights and sizes. We also show that the MPC enables the wheel to accelerate and leverage its inherent braking capability to reach desired speeds—a critical function that did not exist in previous rolling soft systems.

{% include video.html url="//www.youtube.com/embed/o7yJx3-GLs0" %}

## Slides
{: class="no-print"}

The below slides are for the detailed design, modeling, and control of Electrohydraulic Rolling Soft Wheel:
{: class="no-print"}

{% include pdf.html url="portfolio/ElectrohydraulicRollingSoftRobot.pdf" description="" %}