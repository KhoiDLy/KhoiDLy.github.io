---
title: Embedded high voltage power and joystick control of a electro-hydraulic tentacle
# link: https://github.com/scazlab/baxter_collaboration
# link-alt: GitHub repository
img: TerrytheTentacle.jpg
img-thumb: TerrytheTentacle_thumb.jpg
alt: baxter-role-assignment
description: An Easy‐to‐Implement Toolkit to Create Versatile and High‐Performance HASEL Actuators for Untethered Soft Robots
tags: [research,robotics,baxter,hri,human robot interaction,collaborative manufacturing,human robot collaboration,advanced manufacturing,open source,github]
authors: Shane K Mitchell, Xingrui Wang, Eric Acome, Trent Martin, Khoi Ly, Nicholas Kellaris, Vidyacharan Gopaluni Venkata, Christoph Keplinger
submission: Advanced Science, 2019
paper_pdf: "2019_ShaneMitchell_EasyToolkitforHASEL"
paper_title: "An Easy‐to‐Implement Toolkit to Create Versatile and High‐Performance HASEL Actuators for Untethered Soft Robots"
---

With the invention of electro-hydraulic (HASEL) actuators that operate under high voltage, there is an increasing need of miniaturizing embedded high voltage circuit to drive the actuators for robotics applications. Here, we combined a commercial high voltage DC-DC converter (PICO 5VV10P, Pico electronics) and the optocoupler switching circuit from Peta Pico Voltron (https://petapicovoltron.com/) into an H-bridge driver configuration that is often used to control DC motor. This circuit  not only can adjust the high voltage value, but also reverse the high voltage polarity applied to the actuators, thus allowing for improved, robust actuators' performances. The following video provides a more detailed description of the circuit, why high voltage polarity reversal is needed, and how the circuit can be used to drive a soft robotic tentacle.

{% include video.html url="//www.youtube.com/embed/PNgNLz176u0"%}

<!-- ## Method

We target robotic systems that are readily available to non-expert users. In this respect, a **hierarchical task model (HTM)** serves as the entry point for such users: it models the task with the same level of abstraction that one would use to describe the task to another person, while hiding the details of the implementation (cf. Fig. 1).

{% include image.html url="portfolio/BaxterRoleAssignment_htn.png" max-width="80%" description="<b><i>Figure 1</i></b>. HTM for high-level task representation. The user can inspect the task at various levels of granularity, and get feedback from the robot about its estimate of the current subtask (cyan block in picture)." %}

We propose an automated technique able to transform task-level HTMs into low-level on-line planners by using POMDPs. We focus on the optimal exploitation of communication as a (costly) way to reduce uncertainty on the system without affecting its state.
To fulfill this goal, we convert each primitive subtask (that is, each leaf composing the HTM in Fig. 1) into a small, modular POMDP, which we call a **restricted model** (RM [[Shani2014](http://ieeexplore.ieee.org/document/6494590/)], cf. Fig. 2). Hence, the RMs are mostly independent from the rest of the problem and can be studied in isolation. Rach RM is then composed at a later stage and the problem is solved in its entirety. This approach benefits from the modularity of the HTM representation, without the typical sub-optimality of policies that do not consider the full problem.

{% include image.html url="portfolio/BaxterRoleAssignment_htm2pomdp.jpg" max-width="80%" description="<b><i>Figure 2</i></b>. Depiction of the technique used to transform human-readable task models into robot-executable policies. We focus on the optimal exploitation of communication as a (costly) way to reduce uncertainty on the system without affecting its state." %}

## Experiment

In our experiment, the human and the robot are engaged in the joint construction of flat-pack furniture---specifically a stool (cf. Fig. 3).
The metric used to assess the effectiveness of our approach is the _completion time_ that the overall human-robot collaborative system takes to complete the task. We compare our proposed system (**Exp B**) against a control condition (**Exp A**), where the human operator actively asks for specific actions to be performed by the robot through a web interface.
A series of snapshots illustrating the task is shown in Fig. 3.

{% include image.html url="portfolio/BaxterRoleAssignment_snippets.png" max-width="80%" description="<b><i>Figure 3</i></b>. Snapshots acquired during the collaborative assembly of the stool in the control condition (top) and the interactive condition (bottom)." %}

## Results

The framework has been released under the `LGPLv2.1` open-source license, and it is freely accessible on [github.com/scazlab/baxter_collaboration](https://github.com/scazlab/baxter_collaboration) for the Baxter's controllers, and [github.com/scazlab/task-models](https://github.com/scazlab/task-models) for the HTM to POMDP planner.
Although the majority of the codebase is robot-independent, the control architecture is readily available for any Baxter robot.

We test the proposed system in a proof-of-concept scenario in which the human and the robot are engaged in the joint construction of a stool. The system has been evaluated with 8 participants, in a within-subjects design.
Overall, the results suggest evidence of an improvement in terms of task efficiency: two-samples t-test between conditions A and B shows statistically significant difference, with a p-value of `0.016`.

Finally, we have registered a general user preference toward the proposed system. Multiple reasons were given that support the idea that a more transparent interaction favors the collaboration between peers. Most of the comments suggested a reduced cognitive load as the reason for such preference. Please refer to the paper for further information. -->
