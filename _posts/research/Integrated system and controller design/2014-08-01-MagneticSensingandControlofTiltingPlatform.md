---
title: Embedded Magnetic Sensing for Feedback Control of Soft HASEL Actuators
# link: https://github.com/alecive/periPersonalSpace
# link-alt: GitHub repository
img: Tilting_platform.jpg
img-thumb: Tilting_platform_thumb.jpg
alt: Magnetic sensing, control, and tilting platform
description: 6-DOF tilting platform
tags: [research,robotics,icub,robot,humanoids,double touch,self touch,inverse kinematics,denavit-hartenberg,dh parameters,ipopt,optimization,cognitive robotics,body representations,icra,icra 2014,body schema,open source,github]
authors: Vani Sundaram, Khoi Ly, Brian K. Johnson, Mantas Naris, Maxwell P. Anderson, J. Sean Humbert, Nikolaus Correll Mark Rentschler.
submission: IEEE Transactions on Robotics (Submitted in August, 2021)
# paper_pdf: "2014_Roncone_ICRA_kinematic_calibration"
# paper_title: "Electro-hydraulic rolling soft robot: Electromechanical Design, hybrid dynamic modeling, and model predictive control"
---
## Abstract

The need to create more viable soft sensors is increasing in tandem with the growing interest in soft robots. Several sensing methods, like capacitive stretch sensing and intrinsic capacitive self-sensing, have proven to be useful when controlling soft electro-hydraulic actuators, but are still problematic. This is due to challenges around high-voltage electronic interference or the inability to accurately sense the actuator at higher actuation frequencies. These issues are compounded when trying to sense and control the movement of a multi-actuator system. To address these shortcomings, we describe a two-part magnetic sensing mechanism to measure the changes in height of an electro-hydraulic actuator. Specifically, we test our sensing method using folded hydraulically amplified self-healing electrostatic (HASEL) actuators. Our magnetic sensing mechanism can achieve a resolution of <0.1 mm for the HASEL actuator displacement range, and accurately tracks motion at actuation frequencies up to 30 Hz, while being robust to changes in ambient temperature and relative humidity. We successfully perform closed-loop control of one folded HASEL actuator using the sensor. Then, we demonstrate the sensor in a system with six units (one HASEL actuator and one sensor) and control the system to track a desired end effector position in 3D space. This work demonstrates the first instance of sensing electro-hydraulic deformation using a magnetic sensing mechanism. The ability to more accurately sense and control HASEL actuators and similar soft actuators is necessary to improve the abilities of soft, robotic platforms.

## Slides
{: class="no-print"}

The below slides are for the detailed design, characterization and demonstration for control of embedded magnetic sensing:
{: class="no-print"}

{% include pdf.html url="portfolio/MagneticSensingandControlTiltingPlatform.pdf" description="" %}