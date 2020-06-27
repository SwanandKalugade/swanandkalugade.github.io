---
layout: post
title:  CT Fluoroscopy Controller Design
date:   2013-02-20 10:00:00 -0600
category: projects
permalink: /projects/fluoroscopy
image: "/assets/media/fluoroscopy/ctFluoroscopy.png"
---
# Background
CT(Computed Tomography) Fluoroscopy is a useful tool for physicians performing interventional procedures using CT machine. The anomaly in the patient is located with conventional CT imaging, then the physician uses CT fluoroscopy to track the position of a biopsy needle. This controller was a portable device which controlled the CT machine with functions for movement of the couch, gantry and imaging.  

# Brief
The existing product design was two decades old. Canon Medical, Japan wanted to redesign this to offer a new user experience to the user. The key areas were form, usability, ergonomics, and new technology offering flexibility to the product usage.  

# Team
I worked on this project along with my colleagues Mihir Sukhatme (Industrial designer) and Shantanu Rao (Project mentor). We collaborated with Canon Medical team in Japan and Capgemini's product engineering services group.  

# Design Decisions
Ease of operation, sterilization, handling / maintenance and compact footprint were driving points for form consideration. We talked with radiologists, technologists in their work environment to identify pain points and product desirables.  

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
    /* grid-auto-rows: minmax(100px, auto); */
">
    <img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/fieldVisit1.png" alt="Field Visit Japan"/>
    <img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/fluoroscopyDevice.png" alt="Fluoroscopy Device"/>
</div>

> Field visits to University hospital in Tokyo, Japan  


We explored three broad design directions for mounting the controller which provided different affordances. Using cardboard mockups (non-functional prototypes) and role play, we discovered that stand mounted variant seemed cost effective and easy to manage.
<img src="/assets/media/fluoroscopy/Sketches1.png" alt="sketches1" style="border-radius: 0.2em;"/>
<img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/Sketches2.png" alt="sketches2"/>

> Field studies at client site and exploratory sketches in the early stages  

<img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/CT_Mockups.png" alt="mockups"/>

> Idea exploration using traditional as well as digital media  

<br>

# Stand mounted controller
Quick mock-ups with cardboard were used to simulate real environment usage. Testing sessions were conducted in a simulated operating environment to validate human factors. Plastic cover was attached for sterilization as used in a CT scan equipment.  

Several control layout iterations later, two key layouts were selected for detailing.  

<br>

# Selected concepts
<img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/CT_CAD.png" alt="sketches"/>

> Top-Left shows couch / gantry manipulation with physical controls while Bottom-Left moved features to display  

<br>

# SLA mock-up of preferred concept
<img style="border-radius: 0.2em;" src="/assets/media/fluoroscopy/SLA-Mockup.png" alt="sketches"/>

> 1:1 mock-up with simulated materials and colors with GUI on touch-display  

<br>

Two SLA mock-ups were sent to TMSC Japan team for further studies. Capgemini product engineering team continued working on details of the selected concept.
