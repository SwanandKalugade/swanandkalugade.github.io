---
layout: post
title:  Automated Cell Expansion Device
date:   2020-05-18 10:00:00 -0600
category: projects
permalink: /projects/cell-expansion
image: "/assets/media/cell-expansion/quantumSnap.png"
---
*[Quantum](https://www.terumobct.com/quantum "Open Terumo Product Page"){:target="_blank"}* is an automated platform designed to simplify the open, labor-intensive tasks associated with manual cell culture. Although limited in scope for new features, through this project the device will receive updated electro-mechanical components, new display computer, and GUI enhancement.  

# Process
![Whiteboard session](/assets/media/cell-expansion/whiteBoard.jpg)  

After few onboarding sessions, hands-on procedures it became clear that the system uses several pre-defined tasks that can be customized on device. For the design revision, we moved the majority of task / steps creation process to a separate cell processing application. We worked on lots of iterations around providing task customization on device with new Qt framework. 

# Design choices
fontawesome, qt qml types study, adapting common components for devices with resistive and capacitive display, multi-day process where run-screen served as single point of reference, revised accessible color pallete, localization friendly components


#### Modular components
<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cell-expansion/QComponents.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<br>

#### Common components for cell therapy devices
Protocol configuration layout was part of common component for similar projects strategy. We had to update few components for this device's resistive display.  
<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cell-expansion/protocolConfig.mov" type="video/mp4">
  Your browser does not support the video tag.
</video>
<br>

# Localization
<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/cell-expansion/AlterConfigScreen.png" alt="old design">
    <img src="/assets/media/cell-expansion/ICECWashout-German.png" alt="new design">
</div>
<span></span>
> the update offered more space for string expansion within a compact layout

<br>

# Formative testing
We ran the GUI on device's resistive display to test viewing angle, color reproduction, and touch responsiveness.  
<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cell-expansion/cellExpansionDisplayTest.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<br>

The project is in active Qt development phase and will ship to preferred customers in December 2020.