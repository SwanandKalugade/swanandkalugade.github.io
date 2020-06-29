---
layout: post
title:  Cell Processing Device
date:   2020-05-18 10:00:00 -0600
category: projects
permalink: /projects/cps
image: "/assets/media/cps/cellProcessing.png"
---
This new platform combines the capabilities of two existing platforms at Terumo; cell separation, wash and concentrate cells. This device will feature embedded device software and application interface that provides user, protocol and barcode configuration.  

# Process
 

**Protocol configuration**  
All Cell Therapy Technology devices under development at Terumo has similar feature. We were tasked with designing common components that will scale in future, and provide adaptive layout based on xml data.  

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
<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cps/finalRun.mov" type="video/mp4">
  Your browser does not support the video tag.
</video>
<span></span>
> Selected layout scales, localize well, and has touch friendly features for data density

<br>

**Device Run View**  
Device executes different run tasks during a protocol execution. The 'shell' you see below, caters to all possibilities with varying tubing layout connecting bags and pumps, while side panel displays relevant data.  

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
I prepared a quick *[interactive mockup](https://www.justinmind.com/usernote/tests/38196272/45260779/47397928/index.html#/screens/da697580-0312-4404-b07c-5ee3df31b7d4){:target="_blank"}* using JustInMind tool for this study. Some of the views in mockup respond to barcode scan events where I faked them as input events in the tool.  

Systems team worked on protocol steps to perform, arranged disposable tubing kits, a script to simulated alarm lights during workflow execution.  

We received some really great insights into what's important for technicians / nurse during device interactions.  

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

<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cps/hfSession3.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<span></span>

The project is in active Qt development phase and will ship to preferred customers in December 2020.