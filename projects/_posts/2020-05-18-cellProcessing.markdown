---
layout: post
title:  Cell Processing Device
date:   2019-04-20 10:00:00 -0600
category: projects
permalink: /projects/cps
image: "/assets/media/cps/cellProcessing.png"
---
# Background
This new platform combines the capabilities of two existing platforms at Terumo; cell separation, wash and concentrate cells. This device will feature embedded software and application interface that provides user, protocol and barcode configuration.  

# Process
The systems team helped us understand the procedure well through prototype device demos, and documentation. I worked with product owner on the initial explorations, got insights from field clinicians which helped me capture the workflow early on. With subsequent revisions and discovering common features while working on other projects in parallel, we defined ux goals for this project.  

Terumo selected *[Qt Framework](https://www.qt.io/qt-in-medical/ "Open Qt Site"){:target="_blank"}* for its robustness over Chromium browser based GUI. This guided us on feasibility aspect around design of common components.


# Design Choices
FontAwesome icon library with its massive offerings was our choice for interface icons and we created several custom ones in Illustrator. One of the challanging aspect of the project was adapting common components for devices with resistive and capacitive display.  

**Protocol Configuration**  
All cell therapy technology devices under development at Terumo has this similar feature. We were tasked with designing common components that will scale in future, and provide adaptive layout based on xml data.  

Due to data density of task variables and values, we put emphasis on tabular layouts early on but later opted for a card based layout better suited for touch displays.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/PrepareWire1.png" alt="wire1">
    <img src="/assets/media/cps/PrepareWire2.png" alt="wire2">
    <img src="/assets/media/cps/PrepareWire3.png" alt="wire3">
    <img src="/assets/media/cps/PrepareWire4.png" alt="wire4">
</div>
<span></span>
> variety of layout options were tested for ease of use and development

<br>
**Final Layout**
<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/cps/ReviewRun.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<span></span>
> Selected layout scales, localize well, and has touch friendly features for data density

<br>

**Device Run View**  
The cell therapy device executes different run tasks during a protocol execution. The 'shell' you see below, caters to all possibilities with varying tubing layout connecting bags and pumps, while side panel displays relevant data.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/RunWire.png" alt="1">
    <img src="/assets/media/cps/PrimeDesign.png" alt="2" style="border: 1px solid #ECEDED;">
</div>
<br>

# Formative Testing
A JustInMind tool based *[interactive mockup](https://www.justinmind.com/usernote/tests/38196272/45260779/47397928/index.html#/screens/da697580-0312-4404-b07c-5ee3df31b7d4){:target="_blank"}* was used to test user interface during this study. Some of the views in mockup were designed to respond to USB barcode scan events to simulate real world use. Tasks and use scenarios were conveyed to users, and success criteria for user performance was defined by human factors team. Users included nurses, technicians from Europe, China and USA.  

We received some really great insights into what's important for technicians and nurses during these sessions.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/hfSession3.png" alt="1">
    <img src="/assets/media/cps/hfSession2.png" alt="2">
</div>
<span></span>

<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/cps/hfSession3.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<span></span>

The project is in active development phase and will ship to preferred customers in December 2020.