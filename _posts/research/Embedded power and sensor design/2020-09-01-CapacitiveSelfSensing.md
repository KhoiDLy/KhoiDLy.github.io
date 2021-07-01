---
title: Miniaturized capacitive self-sensing for high voltage electrostatic transducers
# link: https://scazlab.github.io/HRC-model-set
# link-alt: webpage
img: CapacitiveSelfSensing.jpg
img-thumb: CapacitiveSelfSensing_thumb.jpg
alt: CapacitiveSelfSensing
description: Miniaturized capacitive self-sensing for high voltage electrostatic transducers
tags: [research,robotics,baxter,hri,human robot interaction,collaborative manufacturing,human robot collaboration,advanced manufacturing,open source,github]
authors: Khoi Ly, Nicholas Kellaris, Dade McMorris, Brian K Johnson, Eric Acome, Vani Sundaram, Mantas Naris, J Sean Humbert, Mark E Rentschler, Christoph Keplinger, Nikolaus Correll
submission: Soft Robotics, 2020
paper_pdf: "2020_KhoiLy_CapacitiveSelfSensing"
paper_title: "Miniaturized circuitry for capacitive self-sensing and closed-loop control of soft electrostatic transducers"
---
Soft robotics is a field of robotic system design characterized by materials and structures that exhibit large-scale deformation, high compliance, and rich multifunctionality. The incorporation of soft and deformable structures endows soft robotic systems with the compliance
and resiliency that makes them well-adapted for unstructured and dynamic environments. While actuation mechanisms for soft robots vary widely, soft electrostatic transducers such as dielectric elastomer actuators (DEAs) and hydraulically amplified self-healing electrostatic (HASEL) actuators have demonstrated promise due to their muscle-like performance and capacitive selfsensing capabilities. Despite previous efforts to implement self-sensing in electrostatic transducers
by overlaying sinusoidal low-voltage signals, these designs still require sensing high-voltage signals, requiring bulky components that prevent integration with miniature, untethered soft robots. We present a circuit design that **eliminates the need for any high-voltage sensing components**, thereby facilitating the design of **simple, low cost circuits using off-the-shelf components**. Using this circuit, we perform simultaneous sensing and actuation for a range of
electrostatic transducers including circular DEAs and HASEL actuators and demonstrate accurate estimated displacements with errors under 4%. We further develop this circuit into a compact and portable system that couples HV actuation, sensing, and computation as a prototype towards untethered, multifunctional soft robotic systems. Finally, we demonstrate the capabilities of our self-sensing design through feedback-control of a robotic arm powered by Peano-HASEL actuators.

{% include video.html url="//www.youtube.com/embed/zd22aOEUt8A" %}

<!-- {% include video.html url="//www.youtube.com/embed/l6alHuMqx6Y" description="Video summary of the proposed work." %} -->


<!-- {% include video.html url="//www.youtube.com/embed/09Zflg7ZzKU" %}


The **Human-Robot Collaboration (HRC) model set** is intended to ease the design of human-robot collaboration experiments.
It targets scenarios like the collaborative assembly of furniture, and consists of a combination of standard components and custom designs, that are:

 * A series of eight 3D printed brackets
 * Dowels
 * Plywood
 * Fasteners (Screws)

The model set aims at reducing the amount of work required to set up and reproduce HRC experiments.
It is designed to be modular, extendable, and easy to distribute. All the content of this repository is distributed under the [Creative Commons attribution-sharealike 4.0 international public license (CC-by-sa)](https://creativecommons.org/licenses/by-sa/4.0/legalcode).

## 3D Printed Brackets

The 3D Printed Brackets were designed with three main criteria in mind : re-use, replicability, and modularity.


The `.stl` files and the SolidWorks files can be found in the [`Bracket STL Files`](https://github.com/ScazLab/HRC-model-set/tree/master/Bracket%20STL%20Files) and [`Bracket SolidWorks Files`](https://github.com/ScazLab/HRC-model-set/tree/master/Bracket%20SolidWorks%20Files) sub-folders respectively.

For more information on how to customize the brackets, please visit [here](https://scazlab.github.io/HRC-model-set/info/how-to-customize/).

## Configurations

We present [four](https://scazlab.github.io/HRC-model-set/configurations/renderings/) prototypical objects built using different configurations of the hardware mentioned above.

Our designs range from the most simple, the Table configuration, to quite complex, the Console configuration.

## 3D Printing

Each bracket is modeled in SolidWorks and then printed on a Dimension Elite FDM printer using ABS+ plastic.

[Here](https://scazlab.github.io/HRC-model-set/info/3D-printing-recommendations/) are some guidelines to use when printing out a file using some common 3D printers. -->
