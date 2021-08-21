---
title: High-bandwidth nonlinear control for soft actuators with recursive network models
# link: https://github.com/alecive/periPersonalSpace
# link-alt: GitHub repository
img: Optical_Block.jpg
img-thumb: Optical_Block_thumb.jpg
alt: High-bandwidth nonlinear control for soft actuators with recursive network models
description: EHigh-bandwidth nonlinear control for soft actuators with recursive network models
tags: [research,robotics,icub,robot,humanoids,double touch,self touch,inverse kinematics,denavit-hartenberg,dh parameters,ipopt,optimization,cognitive robotics,body representations,icra,icra 2014,body schema,open source,github]
authors: Sarah Aguasvivas Manzano, Patricia Xu, Khoi Ly, Robert Shepherd and Nikolaus Correll
submission: International Symposium of Experimental Robotics, 2021
# paper_pdf: "2014_Roncone_ICRA_kinematic_calibration"
# paper_title: "Electro-hydraulic rolling soft robot: Electromechanical Design, hybrid dynamic modeling, and model predictive control"
---
## Abstract

We present a high-bandwidth, lightweight, and nonlinear output tracking
technique for soft actuators that combines parsimonious recursive layers for forward
output predictions and online optimization using Newton-Raphson. This technique
allows for reduced model sizes and increased control loop frequencies when compared with conventional RNN models. Experimental results of this controller prototype on a single soft actuator with soft positional sensors indicate effective tracking
of referenced spatial trajectories and rejection of mechanical and electromagnetic
disturbances. These are evidenced by root mean squared path tracking errors (RMSE)
of 1.8 mm using a fully connected (FC) substructure, 1.62 mm using a gated recurrent
unit (GRU) and 2.11 mm using a long short term memory (LSTM) unit, all averaged
over three tasks. Among these models, the highest flash memory requirement is
2.22 kB enabling co-location of controller and actuator.


## Manuscript
{: class="no-print"}

The below paper is for the detailed description of the neural network architecture for both sensor modeling and controller implementation:
{: class="no-print"}

{% include pdf.html url="portfolio/NeuralControllerforOpticalBlock.pdf" description="This Project describes the Neural controller design for an optical-laced soft robotic block" %}