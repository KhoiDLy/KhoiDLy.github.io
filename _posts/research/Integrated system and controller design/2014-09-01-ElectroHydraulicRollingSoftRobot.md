---
title: Electro-hydraulic rolling soft robot — Design, modeling, and control
# link: https://github.com/alecive/periPersonalSpace
# link-alt: GitHub repository
img: RollingRobot_Sequence.jpg
img-thumb: RollingRobot_Sequence_thumb.jpg
alt: Electro-hydraulic rolling soft robot — Design, modeling, and control
description: Electro-hydraulic rolling soft robot
tags: [research,robotics,icub,robot,humanoids,double touch,self touch,inverse kinematics,denavit-hartenberg,dh parameters,ipopt,optimization,cognitive robotics,body representations,icra,icra 2014,body schema,open source,github]
authors: Khoi Ly, Jatin Mayekar, Sarah A. Manzano, Christoph Keplinger, Mark Rentschler, Nikolaus Correll
submission: IEEE Transactions on Robotics (Submitted in July, 2021)
# paper_pdf: "2014_Roncone_ICRA_kinematic_calibration"
# paper_title: "Electro-hydraulic rolling soft robot: Electromechanical Design, hybrid dynamic modeling, and model predictive control"
---
## Abstract

Rolling robots are attractive due to their simple uniform designs, high degree of mobility, dynamic stability, and self-recovery from collision. In these designs, soft-shell rolling robots are advantageous compared to traditional rigid-shell rolling robots thanks to their ability to absorb and diffuse impact energy upon collision and their conformity to rough terrains. Despite previous efforts to design shell-bulging rolling soft robots, pneumatic and other soft actuators are often limited in terms of high-speed dynamics. Furthermore, mathematical description of the rolling behavior of this type of robot and how these robots can regulate their rolling speed are not mentioned. This paper introduces a cylindrical-shaped shell-bulging rolling soft robot that employs an array of 16 folded-HASEL actuators as a mean for fast and effective rolling. The actuators represent the soft components with discrete forces that propel the robot, whereas the robot's frame is rigid but allows for smooth, continuous change in position and speed. This work discusses the **interplay between the electrical and mechanical design choices, the modeling of the robot's hybrid (continuous and discrete) dynamic behavior, and the implementation of a model predictive controller for the robot's speed.** As a demonstration, we show the robot's ability to **carry integrated hardware (total weight of 0.979 kg) at a maximum rolling speed at 0.7 m/s (1.56 mph),** allowing the robot to outperform the existing rolling soft robots with similar weight and size. Furthermore, the robot's **acceleration and braking are also demonstrated to track real-time referenced speeds** with satisfactory performance.

{% include video.html url="//www.youtube.com/embed/o7yJx3-GLs0" %}

## Slides
{: class="no-print"}

The below slides are for the detailed design, modeling, and control of Electrohydraulic Rolling Soft Robot:
{: class="no-print"}

{% include pdf.html url="portfolio/ElectrohydraulicRollingSoftRobot.pdf" description="" %}