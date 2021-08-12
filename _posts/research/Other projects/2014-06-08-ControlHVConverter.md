---
title: Digital Control of HV DC-DC Converter
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

## Description

The presented HV DC-DC converter (EMCO Q101) is a proportional, unregulated converter that can amplify an input voltage between 0 - 5 V to 0 - 10 kV. However, the device's output voltage is load dependent. The goal of this project is to design a step-up DC-DC converter, implement a lead-lag compensator to control the voltage output of the converter irrespective of the load.

To obtain the dynamic model of a commercial device, we employed a system identification technique called chirp response. Based on the frequency response of the converter, a single input - single output (SISO) transfer function of the device can be obtained. The model of the step-up DC-DC (buck) converter that drives the HV DC-DC conveter is well-known and can be obtained from any power-electronic textbook.

Based on the combined model of the two converters, the Nyquist and Root Locus techniques can be used to determine the poles and zeros location of the closed loop system. This analysis allows for the stability of the controller and improved response time of the converters.

The results, measured by a high voltage probe, are presented in slide 12. The ripple noise of the HV converter is intrinsic to the HV converter and is independent from the controller; the steady-state HV outputs are satisfactory with different loads.

## Slides
{: class="no-print"}

The below slides are from the digital Control Final Project 2018:
{: class="no-print"}

{% include pdf.html url="portfolio/Control_HV_DCDC_Converter.pdf" description="Course Project in Digital Control 2018" %}