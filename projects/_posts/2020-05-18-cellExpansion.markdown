---
layout: post
title:  Automated Cell Expansion Device
date:   2019-02-10 10:00:00 -0600
category: projects
permalink: /projects/cell-expansion
image: "/assets/media/cell-expansion/quantumSnap.png"
---
# Background
*[Quantum](https://www.terumobct.com/quantum "Open Terumo Product Page"){:target="_blank"}* is an automated platform designed to simplify the open, labor-intensive tasks associated with manual cell culture. Through this enhancements project the device will receive updated electro-mechanical components, new display computer, and GUI refresh.  

# Process


![Whiteboard session](/assets/media/cell-expansion/whiteBoard.jpg)  

We did iterations to provide task customization on device with new Qt framework. The device typically has multi-day process where run-screen serves as a single point of reference. We reworked Terumo's accessible color pallete especially for this.  

# Design choices
It became clear that the system uses several pre-defined tasks that can be customized on device. For the design revision, majority of task / steps creation process was ported to a separate cell processing application.  

**Modular Components**  
To solve string expansion, repond to user entries, and device states, we spent more time on modular components. Using Qt's Sketch Plugin, we were able to export ui.qml files for the developement team. This ensured there's little loss while translating design intent into development.  

<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/cell-expansion/modularQuantum.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<br>

**Common Components for Cell Therapy Devices**  
Protocol configuration layout was part of common component for similar projects strategy. We had to update few components for this device's resistive display.  
<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/cell-expansion/config.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<br>

# Localization
Terumo devices get localized into various languages including EMEA, CJK etc. We worked with l10n team closely to avoid any issues leaking into development.  
<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/cell-expansion/AlterConfigScreen.png" alt="old design" style="border: 1px solid #ECEDED;">
    <img src="/assets/media/cell-expansion/ICECWashout-German.png" alt="new design" style="border: 1px solid #ECEDED;">
</div>
<span></span>
> the update offered more space for string expansion within a compact layout

<br>

# Formative testing
We took the finished version of the GUI and ran it on the device's resistive display to test viewing angle, color reproduction, and touch responsiveness. This was valuable both to design, and development team.  
<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/cell-expansion/cellExpansionDisplayTest.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
> Initial version for enhancements was targeted at capacitive display but increased cost in tooling required to update display mounting changed the tech back to resistive type  

<br>

The project is in active development phase and will ship to preferred customers in December 2020.