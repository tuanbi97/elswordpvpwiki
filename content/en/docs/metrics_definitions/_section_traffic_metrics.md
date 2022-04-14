---
title: "Section Traffic Metrics"
linkTitle: "Section Traffic Metrics"
weight: 4
description: >
  All metrics related to section level traffic data.
---

## Section Visits
**Definition**: Number of unique customers to a section.

**Other Names**: Section Footfall

### How It is Measured
We define sections as areas in camera as below: 
<img src="https://storage.googleapis.com/palexy-static-files/documents/section_drawn_on_camera.png"/>

Everytime a customer walks into the defined area and stays for more than 30 seconds, we consider it as a visit to that section. 

In the same store visit session, if the customer leaves the section then comes back, we will not count the second visits since we are counting unique visits to a section. 


## Section Visit Rate
**Definition**: Percentage of store customers who visit the section. `Section Visit Rate = 100% * Section Visits / Store Visits`

## Section Average Dwell Time
**Definition**: Average amount of time customers stay in the section in seconds.

