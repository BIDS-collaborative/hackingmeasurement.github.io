---
title: Urthecast and Semester Review
author: Dav Clark, Joris Ramstein, Hans Lui
presenters:
layout: class
---

## Announcement

Check out these [presentations from DIL
postdocs](http://dil.berkeley.edu/event/development-engineering-lessons-from-the-dil-postdocs/)
for more inspiration at 4pm after class!

## Reading / Tech

Please review our very own [project pages](/projects.html)!

## Tentative plan

First, Catherine Burton from Urthecast will give us a brief overview of earth
observation satellites, remote sensing image processing, machine learning
algorithms, APIs and the advent of big data analytics and unstructured data.

**Then we'll have class review!**

Then, we'll have a lively review of the semester. If a team can't make it for
the final presentations, this is an alternative date. Teams on deck so far:

- CEGA-trace
- The Carpool Project



----------------------

##The carpool project

- has been working on this for a year
- charge riders to get from a to b and pay riders
- different scales
- mobile product was also designed
- hit a wall when thinking of the end-user service

Data project evolved; challenges:
- how do we enlist people and collect mobility data
-> solution: development of a userguide
- app needs to be downloaded
- user needs to understand it is private, all about saving money, time and the planet!

Currently, the data collection has to be done as a 2-step process:
- people have to download the moves app
- people have to export data to local device then send it over
—> Reprocessing needed to be done

- How do we figure out that people have common routes?
- configured a time window (within 10, 15 30 minute intervals)
- then subclassifications within walking distance/time to walk
- then take longest trip from subclassifications, assume they start from the same location and make the classification more specific

Overall goal is to reduce competitive ride-sharing apps prices by reducing ride costs to a fraction of the competitive prices, even if that means walking 20 minutes for the rider.

##Earth observation and big data analytics (Catherine Burton)

Background in geospatial analytics
“Urthecast” : They have 4 satellites, including a color live camera

Remote sensing: the process of obtaining information about an object and gathering data from a sensor from a distance

The technology started during the war, cameras were strapped to pigeons or balloons

1946: first image taken from a rocket
1960: first meteorological satellite
1960-72: spy satellite program
1972: first civilian land satellite
1999: first high resolution image satellite

Different technologies

NASA’s EO (earth observation) system
- LOTS of satellites
- images can found on earth explorer; any given location every 16 days

Aerial photography:
- lots of pictures for one location
- VERY high resolution (3 inches/pixel!)

Kite photography:
- pictures need to be patched together into a final image
- VERY cheap
- Drones are the new thing

LiDAR
- creates a 3D point cloud, flown from a plane
- uses light data

SAR (synthetic aperture radar)
- advantage: can go through clouds
- sound-based (more like a sonar)
- “holy grail” application of SAR: being able to find ships

Measuring the Earth with sensors
- Natural entities can be measured using different electromagnetic frequencies
- satellite can be trained to recognize different wavelengths of the EM spectrum
- vegetation health, water levels, melting ice caps etc. can all be measured!

how to visually interpret satellite imagery?
- each raw image has pixels, each with an intensity value
- supervised and unsupervised analysis
- tone and color
- size and shape
- texture and pattern
- location and features

The four V’s of big data:
Volume
Velocity
Variety
Veracity

Geographic Information Systems (GIS)
- information system that integrates, stores, edits, analyzes, shares and displays geographic information
- tools that allow users to create interactive queries
- Big data on the other hand is a broad term for data sets so large or complex that traditional data processing applications are inadequate

Big data and IoT have been merging together

Pattern recognition: algorithms apply some filters to an image and apply morphological recognition
Machine learning: algorithms aimed at prediction of data beyond recognition only
Deep learning: algorithms extract high level complex abstractions as data representations through a hierarchical learning process