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
## Abstract

Soft robotics is a field of robotic system design characterized by materials and structures that exhibit large-scale deformation, high compliance, and rich multifunctionality. The incorporation of soft and deformable structures endows soft robotic systems with the compliance
and resiliency that makes them well-adapted for unstructured and dynamic environments. While actuation mechanisms for soft robots vary widely, soft electrostatic transducers such as dielectric elastomer actuators (DEAs) and hydraulically amplified self-healing electrostatic (HASEL) actuators have demonstrated promise due to their muscle-like performance and capacitive selfsensing capabilities. Despite previous efforts to implement self-sensing in electrostatic transducers
by overlaying sinusoidal low-voltage signals, these designs still require sensing high-voltage signals, requiring bulky components that prevent integration with miniature, untethered soft robots. We present a circuit design that **eliminates the need for any high-voltage sensing components**, thereby facilitating the design of **simple, low cost circuits using off-the-shelf components**. Using this circuit, we perform simultaneous sensing and actuation for a range of
electrostatic transducers including circular DEAs and HASEL actuators and demonstrate accurate estimated displacements with errors under 4%. We further develop this circuit into a compact and portable system that couples HV actuation, sensing, and computation as a prototype towards untethered, multifunctional soft robotic systems. Finally, we demonstrate the capabilities of our self-sensing design through feedback-control of a robotic arm powered by Peano-HASEL actuators.

{% include video.html url="//www.youtube.com/embed/zd22aOEUt8A" %}

## Slides
{: class="no-print"}

The below slides are for the detailed design, characterization, and application of the miniaturized capacitive self-sensing technique for electrostatic actuators:
{: class="no-print"}

{% include pdf.html url="portfolio/CapacitiveSelfSensing.pdf" description="This Project describes the capacitive self-sensing technique" %}