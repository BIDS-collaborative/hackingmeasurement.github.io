---
title: Launch Meeting
author: Dav Clark
layout: meeting
---
## In attendance

 - Falk Schustenmeyer (CNR, Ecoengine, BIDS)
 - Dav Clark (D-Lab, BIDS)
 - Guillaume Kroll (CEGA / BITSS)
 - Javier Rosa (TIER / Mezuri)
 - Sidney Alexander Feygin (EECS)

## Agenda

Introduce likely core content contributors, discuss plans for the semester.

## Tentative plan (from Dav)

I'm not sure if we should shoot for 2 or 3 seminars this semester. As you can
see, I'm still finding out about finances. But at a minimum, I'd love to do
these two:

1. A seminar focused on mobile (android-focused, but at least touching on what
   you'd do for iOS or cross-platform). Javier, I'm hoping you'd take the lead
   on at least determining content of that seminar (so that we are coherent with
   the directions Mezuri is going), with support from Sid.

2. A seminar focused on sensors. I'm working with a guy from the GIF on
   environmental sensing, and we're instrumenting environmental and social
   sensing in the BIDS space. It'd be great to come up with a cross-disciplinary
   list of examples, along with basic pointers on how to get started, or
   integrate with existing units on campus. We might also reach out to folks on
   campus like the nano-lab or whoever else works on mobile / embedded
   electronics.

Other topics could include remote sensing, datasets such as the call data record
and micro-grid data from TIER, and inviting some folks in to talk about 3D (or
4D) capture.

I wanted to reach out to you three first, but I'd like to establish the core
team that's going to have input.

We also discussed making this website!

## Notes from Sid

I’m happy to provide insight on my experience integrating funf in our upcoming
mood and decision-making study, mobile programming in general as well as
ODK-related matters. I also now have some experience with call data record
research through our SmartBay microsimulation work. W/R/T mobile I can think of
a few salient topics to cover:

+  Multipurpose Interdisciplinary Studies:
    - While including an economist did necessitate additional software
      engineering, the benefits of including a social scientist directly in the
      project team outweighed the costs. The benefits included additional
      funding, experience w/ IRB procedures, and insight into experiment design. 
    - Through our colleagues, we’ve secured access to additional data that
        seems compatible with the goals of our study. Facilitating these sorts
        of data sharing agreements seems to be something BIDS could take a
        leadership role in.

+ User Retention and Design Issues:
    - While the goal for the scientist is data collection, the user must remain
      engaged with the app through the study period. This necessitates insight
      from HCI specialists, or at least concern for externalities of data
      collection such as battery-life, resource sharing, and understanding of
      basic UI/UX heuristics.
    - Like any application, experimental procedures should allow comfortable
      time for design lifecycle stages such as prototyping and pilot-testing.
    - W/r/t software engineering, a focus on modular design and integration of
      existing libraries will improve code reuse and reduce development burden
      (note <http://android-arsenal.com> for a huge repository of libraries and
      example applications for Android.)
    - Cross-Platform vs. Native solutions. Multi-platform teams, etc.

+ Data Quality:
    - Top priority for scientists and requires the most direct interaction w/
      software engineers.
    - From experience, researchers should be responsible for defining,
      communicating, and accepting data quality criteria prior to experiment
      trial (!)
    - During the experiment, data should be frequently assessed, EDA techniques
      established, and abnormalities noted to tech team.

I can go over other stuff as well, but these are the first things that come to
mind.

emote/Environmental Data Provenance Infrastructure:
<https://wq.io/media/papers/provenance_cscw14.pdf> (Bonus: Implemented in Django!)

Open mHealth: <http://www.openmhealth.org/our-approach/clinical-schemas/>
(description of their approach to data schematization)

funf: <http://www.funf.org/> (pluggable behavioral sensing toolkit… see
“developers". Note that 0.5 RC1 is a bit buggy, which is why we decided to go
with 0.4.2. There are major benefits to 0.5, but it’s not supported, and, though
I think I worked out most of the issues, I didn’t feel safe integrating it into
a production app).

Innovative human research metadata privacy infrastructure:
<http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098790> (from
De Montjoye)

## Slack

Dav created a chat room in the "Moore-Sloan Data Science Environment" for
tech4measurement. Dav thinks the main idea is that we could discuss issues that
folks are currently concerned about in BIDS - surrounding surveillance and how
to protect subjects (esp. when the subjects are "us"). You are invited to join
as well - ideally we'll get some cross-campus support around this topic:

<https://msdse.slack.com/messages/tech4measurement/>

If you're not interested in joining, no worries - and you can always join later!
