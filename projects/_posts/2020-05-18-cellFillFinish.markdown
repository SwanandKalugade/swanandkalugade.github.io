---
layout: post
title:  Cell Therapy Device
date:   2020-05-18 10:00:00 -0600
category: projects
permalink: /projects/ctt
image: "/assets/media/cell-therapy/cellFillFinish.png"
---
# Background
Cell therapy manufacturing is a complex, multi-step process that takes place at various locations. But in general, cell therapy labs show an overall low level of automation throughout all regions.

This device is the first device of its kind to automate the final steps of cell and gene therapy manufacturing process, while help facilitate cGMP compliance. It is a functionally closed system for cells that automates mixing, cooling, air removal, aliquoting and sealing.  

# Brief
The operator should follow the guided on-screen instructions to load the tubing set, enter processing data, customize parameters, connect the material to the tubing set, and perform and troubleshoot the procedure on the device.  

# Process
![ux process](/assets/media/cell-therapy/UX Process.png)  
> UX ownership with responsiblities in overall project execution  

#### Theme selection
Terumo's Dark UI Theme is high contrast and industrial looking that follows best practices on creating a highly-visible and efficient interface. The GUI compliments device's black display housing. This creates a familiar and consistent user experience pulling inspiration from other laboratory and medical device UIs.  

#### Wireframe to Design
From initial ideations to designs for production, the user interface evolved quite a lot. This is mostly due to field study insights from service engineers and formative testing sessions.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/cell-therapy/finiaWire.png" alt="cellTerapy Balsamiq">
    <img src="/assets/media/cell-therapy/FINIAEarly.png" alt="diagram Early">
    <img src="/assets/media/cell-therapy/loadTubing.png" alt="load Tubing Diagram">
</div>
<span></span>
> A workflow sample showing transition from simple wireframes to subsequent refinements in design

#### Localization aspect
Terumo's localization and tech-comm team has defined best practices for GUIs. They also review all UI designs to ensure strings can scale well, word-wrap, and convey right meaning in different languages.  
<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/cell-therapy/l10n2.png" alt="l10n comments">
    <!-- <img src="/assets/media/cell-therapy/l10n.png" alt="l10n remarks"> -->
</div>
<span></span>  

#### Proposed library
Due to its robustness, official library for Angular, a non-proprietary industry standard was used for front-end development.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/cell-therapy/angularMaterial.png" alt="angular material">
    <img src="/assets/media/cell-therapy/materialSpec.png" alt="material spec">
</div>
<span></span>
> Angular material provides components, transitions, grid system, and allows for robust theming.   

This worked for this project but few months later for another graphically demanding project we found out that Chromium on device is not as robust as desktop or mobile experience. As of 2020 team shifted its focus to Qt Quick GUI framework instead, which gives a compiled application to deploy and is provides smoother experience.

#### Prototype


<br>
# Product demo
<iframe 
    width="100%" 
    height="400" 
    src="https://www.youtube.com/embed/whrMosfqfTU?fs=0&mute=1" 
    frameborder="0" 
    allow="accelerometer; encrypted-media; gyroscope;">
</iframe>  

> first of its kind device to automate final formulation and fill and finish for cell therapy manufacturing
