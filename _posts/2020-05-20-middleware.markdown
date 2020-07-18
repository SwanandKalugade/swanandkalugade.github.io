---
layout: post
title:  Solution for Ortho Diagnostics
date:   2020-05-20 09:10:00 -0600
category: posts
permalink: /posts/middleware
---
## Background
<div style="margin-bottom: -0.8em;"></div>
Ortho Diagnostics plans to develop a next generation Donor Screening solution. This middleware shall centralize the multi-instrument result handling database, and interface to the customer’s Lab Information System (LIS). Instrument and LIS communications will utilize HL7 communications format. 

<mark style="background-color: #FFDF7F;">This recent work below in brief was part of Capgemini's proposal response for Ortho Diagnostics.</mark>

## User Journey Map
### Scenario
The Lab Technician has privileged access and expected to track the instrument status, condition codes triggered, monitor system operations, and generate status reports.
<div style="margin-bottom: -0.8em;"></div>
<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
">
    <img src="/assets/media/middleware/journeyMap.png" alt="user journey map"/>
</div>

## Design
After studying high level feature requirement, I sorted the common features together. We worked on two personas that will use this tool for different purposes. A dashboard view was added to provide a snapshot of key metrics for the admin.

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
">
    <img src="/assets/media/middleware/Map.png" alt="user journey map"/>
</div>

# Features Covered
1. **Dashboard** > Representation of key metrics important to Admin and can be exposed to other users with permissions, if necessary. Users can pick from pre-defined metrics, define custom view of metrics on Dashboard. Other relevant data / links can be added to dashboard. Users can hot-link to other sections in the application from these metrics.
2. **Monitoring > Instrument status view** for Admin, who can filter it out based on site the instrument is at, it's status (online/offline/in-use/no license). User can hot-link to order#, result flags and records. User can dig into an Instrument from list of Instruments, available at their health-care facility. May provide feature to configure devices from this view.
3. **Users > ‘Local’ users** are those created in the middleware database, whereas ‘Imported’ are from Active Directory. Admin can assign site access and roles to individuals and add their details.
4. **Configuration-Authentication > Middleware** softwares' session timeouts, AD source.
5. **Configuration-Network > IP settings** for middlewares' connection to network, destination for e-Connectivity portal at Ortho Diagnostics. There could be other sub-sections within Configuration like, Language packs, Printer setup.

<div style="margin-bottom: 2em;"></div>

<video width="100%" height="auto" controls muted style="border: 1px solid #ECEDED;">
  <source src="/assets/media/middleware/middleSol.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<br>
<div style="margin-bottom: -1em;"></div>

# Usability Considerations
1. UI widgets shall scale with string widths during l10n (localization) or can be adjusted to support varying common screen sizes.
2. UI is influenced by Google’s Material Design system but customized as per Ortho’s branding.
3. Charts / Metrics color palette, charts are opinionated to match Ortho branding.
4. Gray UI palette is intentional and presents content first while keeping branding subtle.
5. UI widgets showcased pass colorblind simulation tests for charts, input statuses, current selection and can be improved with field insights.
6. App logo can be customized to the facility where software will be consumed at.