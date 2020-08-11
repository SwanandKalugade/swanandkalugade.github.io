---
layout: post
title:  Redesign of CT Fluoroscopy Controller
date:   2014-05-18 10:00:00 -0600
category: projects
permalink: /projects/fluoroscopy
image: "/assets/media/fluoroscopy/ctFluoroscopy.png"
---
# Background
CT(Computed Tomography) Fluoroscopy is a useful tool for physicians performing interventional procedures using CT machine. The anomaly in the patient is located with conventional CT imaging, then the physician uses CT fluoroscopy to track the position of a biopsy needle. 

For a physician, this controller augments CT machine functions like movement of the couch, gantry, and imaging while operating on a patient.

<br>

# Brief
Cannon Medical's CT controller was two decades old design. They saw this project as an opportunity to offer a new user experience. The key design considerations were form, usability, ergonomics, and new technology offering flexibile usage.

My ID colleagues and I worked together on this project with Canon Medical team in Japan and Capgemini's product engineering services group.

<br>

# Design Choices
Form considerations included ease of operation, sterilization, maintenance, and compact footprint. We consulted radiologists, technologists in their work environment to identify pain points and product desirables.

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img src="/assets/media/fluoroscopy/fieldVisit1.png" alt="Field Visit Japan"/>
    <img src="/assets/media/fluoroscopy/fluoroscopyDevice.png" alt="Fluoroscopy Device"/>
</div>
<span></span>
> Field visit to University hospital in Tokyo, Japan

<br>
We explored three broad design directions for mounting the controller which provided different affordances. Using cardboard mockups (non-functional prototypes) and role play activities, we discovered that the stand mounted variant seemed cost effective, easy to install and manage.
<img src="/assets/media/fluoroscopy/Sketches1.png" alt="sketches1"/>
<img src="/assets/media/fluoroscopy/Sketches2.png" alt="sketches2"/>

> Field studies at client site and exploratory sketches in the early stages  

<img src="/assets/media/fluoroscopy/CT_Mockups.png" alt="mockups"/>

> Idea exploration using traditional and digital media  

<br>

# Stand mounted controller
We conducted testing sessions using cardboard / foam mock-ups in a simulated operating environment to validate human factors. The test included double gloved operation with plastic cover on controller for sterilization, as used in a CT scan environment.  

Two key layouts were selected for detailing after going through several control layouts.

<br>

# Selected concepts
<img src="/assets/media/fluoroscopy/CT_CAD.png" alt="sketches"/>

> Top-Left image shows couch / gantry manipulation with physical controls while Bottom-Left shifted features to the display

<br>

# SLA mock-up of preferred concept
<img src="/assets/media/fluoroscopy/SLA-Mockup.png" alt="sketches"/>

> 1:1 mock-up with simulated materials and colors with GUI on touch-display 

<br>

For further studies, two SLA mock-ups were sent to Canon Medical Japan team. Capgemini product engineering team later continued working on details of the selected concept.