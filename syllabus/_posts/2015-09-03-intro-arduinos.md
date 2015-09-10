---
title: Intro to Arduinos, Collaborative Projects
author: Dav Clark
presenters: Javier Rosa
layout: class
---
## Announcements

Upcoming events at [ManyLabs](https://www.manylabs.org/):

 - Work party this coming Thursday, September 10 from 4-6 PM [at
   ManyLabs](https://www.google.com/maps/place/Manylabs/@37.777164,-122.407709,17z/data=!4m3!3m2!1s0x80858082235da2e7:0xb30be4b717ffde73!4b1).
   We will be building plant boxes for 2nd graders that will be rolled from the
   exhibit space to outside.
 - Stay tuned for more exciting events!

## Kick-starting team formation

We'll circulate through the room, and start assigning folks to teams. We'll
have facilitators organizing the projects throughout the room.

Dav:

 - BIDS Guests
 - Ecostations Data Access Monitor (EDAM)
 - HOLOS / EcoEngine (preview, but no specific project yet)
 - ODK contributions
 - Clinton Global Health Access (preview, specific projects en route)
 - Primary education tutoring

Temina:

 - BITSS open data audit
 - CEGA impact

Anthony:

 - Aurorasaurus for protest observation
 - Berkeley seismology visualizations
 - ManyLabs air quality sensors
 - (John Naulty if in the room) NeurotechX (preview, pending specific project)

## Arduinos as a basic platform


### Reading / Tech

You are highly encouraged to buy your own Arduino and related electronics!
However, we will provide teams of 2-4 with sufficient materials to complete all
projects. A shopping list will be provided.

Please read up on arduinos on the internet. Keep track of interesting URLs you
find. Good places to start are adafruit and sparkfun (they will also try to
sell you things).

### Tentative plan

 - Intro to sensor-based projects
    - GPS monitoring of water collection habits
    - Temperature monitoring of cookstoves
    - Combined sensor and actuation to implement a demand response system
    - Air quality (cf. Greg Neimeyer, Peter Sand, Matt Gee)
 - What's a microcontroller?
    - Why Arduinos
    - What else might you use?
 - What sensors are available
    - Trip sensors
    - Switches
    - Transducers (light, sound, pressure)
    - Open Energy Monitor (an open source power monitoring project)
    - Flexbox project 
    - Clamp sensors to measure current

---

## Notes from Class

Second meeting: 2015-09-03.

## Agenda

* Announcements
* Projects/team formation

### Announcements

**Get on [Gitter](gitter.im/BIDS-collaborative/hackingmeasurement.github.io)**.

* At the bottom of the [class site](j.mp/HMclass15), there is a link for joining Gitter

There are upcoming events at [ManyLabs](https://www.manylabs.org/). ManyLabs is like a tech shop/hacker space around science and education.

* Plant boxes for 2nd graders in SOMA
* Nerds for Nature Hackathon

Course Entry Codes handed out today.

### Teams

#### Established projects

There are about 10 projects groups can choose to work on.

* Campus Pass System
* OpenDataKit
* Aurorasaurus for Protest Observation
* NeurotechX
* Air Quality Sensors with ManyLabs
* Earthquake Measurement and Visualization
* Ecostation Data Access Monitor
* Auditing Open Data Publications with BITSS
* Conflict Monitoring

More details [here](http://hackingmeasurement.berkeley.edu/projects.html).

For teams, the following are needed:

* Team lead
* 

To make serious progress, you'll want about 10 hours a week. Not everyone has to commit to this level, though. Think about: how to make it the best experience for yourself; setting up project goals and timeline.

Each group will have a mentor: clients or BIDS Fellows.

Student comment: for each project, it would be nice to know the expectations.

#### Other projects

**Vivek**. Doubling the occupancy of all vehicular traffic. "An Uber for drivers." Do the reverse of what Uber does. Match riders to all of the cars driving around. "Can cut the cost of a ride by 10." Goal: save everybody money, perhaps time, and carbon emissions. Existing app, Move, tracks locations and means (biking, walking, etc.). The hard problem is a data science problem: what should the footprint be for adoption, the go-to-market strategy?

## Building Sensors

With Javier, Technology and Infrastructure for Emerging Regions (TIER).

### Why sensors?

### Sensor Ecosystem

Sensors, gateways, and examples.

Non-obvious things:

* Matching identifiers
* Maintenance

Lots of sensors available for the class. If you think you need to measure something, speak with Dav and/or Javier.

Mobile phones are getting a lot cheaper and have lots of sensors built in:

* Accelerometers
* Compass
* Gyroscope
* Bluetooth
* WiFi
* GPS
* Light Sensor
* Camera
* Capacitive Touch
* Temperature

Examples of what you can measure with sensors

* Motion or Activity
* People
* Air
* Water

Motion or activity. Interesting use of accelerometers: measure whether or not lighting changing walking speed.

Arduino: a "microcontroller" that runs your code directly, giving direct access to hardware (no operating system).

Raspberry Pi:

BeagleBone: can be used as a gateway

### Cookstoves

To get a sense of how often people use cook stoves and for how long, iButton temperature sensors can be used.

For a lot of social science projects, you're not only monitoring physical things, you're also asking people questions.

### FoneAstra

Can keep track of time. Most systems don't have this capability, unless connected to a network.

Used for the Milk Bank project: interfaced with the phone and could monitor pasteurization of milk.
