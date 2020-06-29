---
layout: post
title:  Cell Processing System
date:   2020-05-18 10:00:00 -0600
category: projects
permalink: /projects/cps
image: "/assets/media/cps/cellProcessing.png"
---
This new platform combines the capabilities of two existing platforms at Terumo; cell separation, wash and concentrate cells. This device will feature embedded device software and application interface that provides user, protocol and barcode configuration.  

# Design

All Cell Therapy Technology devices under development shared this feature. We were tasked with designing common components that will scale in future, and provide adaptive layout based on xml data.

#### Example 1
We went through several layout options for protocol configuration view below. Due to data density of task variables and values, we explored tabular layouts  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/PrepareWire1.png" alt="1">
    <img src="/assets/media/cps/PrepareWire2.png" alt="2">
    <img src="/assets/media/cps/RunXD2.png" alt="3">
    <img src="/assets/media/cps/RunXD.png" alt="4">
</div>
<span></span>

<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cps/finalRun.mov" type="video/mp4">
  Your browser does not support the video tag.
</video>
<span></span>
> Selected layout scales, localize well, and has touch friendly features for data density

<br>

#### Example 2
<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/RunWire.png" alt="1">
    <img src="/assets/media/cps/PrimeDesign.png" alt="2">
</div>
<span></span>


# Human factors session
Alongwith the systems team at Terumo, I worked on a quick interactive mockup using JustInMind tool. Systems folk worked on protocol steps to perform, arranged disposable tubing kits, a script to simulated alarm lights during workflow execution.  

We got some really great insights into how technicians / nurses wanted from the device interactions.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
">
    <img src="/assets/media/cps/hfSession1.png" alt="1">
    <img src="/assets/media/cps/hfSession2.png" alt="2">
</div>
<span></span>

<video width="100%" height="auto" controls muted>
  <source src="/assets/media/cps/hfSession3.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>