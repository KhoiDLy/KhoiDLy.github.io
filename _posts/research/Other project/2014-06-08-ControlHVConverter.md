---
title: PID Control of HV DC-DC Converter
# link:  http://www.icub.org/other/icdl-epirob-2014/dbr_workshop.html
# link-alt: website
img: HV_DCDC_Converter.jpg
img-thumb: HV_DCDC_Converter_thumb.jpg
# alt: Embedded Magnetic Sensing for Feedback Control of Soft HASEL Actuators 
# description: Half-day workshop at ICDL-EPIROB 2014 Conference
# tags: [research,robotics,baxter,hri,human robot interaction,collaborative manufacturing,human robot collaboration,advanced manufacturing,open source,github]
# authors: Vani Sundaram, Khoi Ly, Brian K. Johnson, Mantas Naris, Max Anderson, J. Sean Humbert, Nikolaus Correll, Mark Rentschler
# submission: Soft Robotics 2020
# paper_pdf: "2020_KhoiLy_CapacitiveSelfSensing"
# paper_title: "Miniaturized circuitry for capacitive self-sensing and closed-loop control of soft electrostatic transducers"
---


<!-- We believe the transition from robots as recipients of human instruction to robots as capable collaborators hinges around the implementation of **transparent systems**, where mental models about the task are shared between peers, and the human partner is freed from the responsibility of taking care of both actors.
In this work, we implement a transparent task planner able to be deployed in realistic, near-future applications. The proposed framework is capable of basic reasoning capabilities for what concerns role assignment and task allocation, and it interfaces with the human partner at the level of abstraction he is most comfortable with. The system is readily available to non-expert users, and programmable with high-level commands in an intuitive interface. Our results demonstrate an overall improvement in terms of completion time, as well as a reduced cognitive load for the human partner.

## Description

This project deals with the task of solving the problem of _self-(or double-)touch_. It is defined as the robot being able to touch itself on a specific region of the skin, and it represents an unprecedented opportunity for a humanoid robot to achieve the simultaneous activation of multiple skin parts (in the video above, patches belonging to the right hand and the left forearm). This high amount of information is then used for a completely autonomous calibration of the body model (i.e. kinematic calibration or tactile calibration).

The _self-touch_ or _double-touch_ scenario has been further exploited for collecting tactile and proprioceptive data that serve kinematic calibration. In robotics, this constitutes a novel solution to the problem, in that no external metrology (like cameras or other tracking apparatus) is necessary. The kinematic chain is closed through touching its own body: the correspondence between the predicted contact point from existing forward kinematics and the actual position on the robot's "skin" provides sample data that allows simultaneous learning of the kinematic representation as well as the position of individual tactile sensors (taxels). The existing iCub kinematic model (DH parameters) and initial calibration of the tactile array serves as a starting point and we have successfully improved on these. The data collection procedure is automated - self-touch is autonomously executed by the robot - and can be repeated at any time, providing a compact self-calibration system.

At present, the visual modality is being added, employing modules that already exist for the iCub (object tracking, gaze controller, stereo vision). This will allow for automatic calibration of additional components of the system: head and eye kinematics, the stereo pair, and camera projective maps. Furthermore, in collaboration with Bielefeld University, we are improving the autonomy and robustness of the double-touch behavior by using visual and tactile servoing.

## Slides
{: class="no-print"}

Here are the slides I used during the presentation at ICRA2014:
{: class="no-print"}

{% include pdf.html url="portfolio/doubleTouch.pdf" description="Slides used at ICRA2014" %}

## Paper Abstract

Calibration continues to receive significant attention in robotics because of its key impact on performance and cost associated with the operation of complex robots. Calibration of kinematic parameters is typically the first mandatory step. To this end, a variety of metrology systems and corresponding algorithms have been described in the literature relying on measurements of the pose of the end-effector using a camera or laser tracking system, or, exploiting constraints arising from contacts of the end-effector with the environment.
In this work, we take inspiration from the behavior of infants and certain animals, who are believed to use self-stimulation or self-touch to “calibrate” their body representations, and present a new solution to this problem by letting the robot close the kinematic chain by touching its own body. The robot considered in this paper is sensorized with tactile arrays for a total of about 4200 sensing points. The correspondence between the predicted contact point from existing forward kinematics and the actual position on the robot’s ‘skin’ provides sample data that allows refining the kinematic representation (DH parameters). The data collection procedure is automated — self-touch is autonomously executed by the robot — and can be repeated at any time, providing a compact self-calibration system that does not require an external measurement apparatus. -->
