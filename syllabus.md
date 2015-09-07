---
title: Syllabus
author: Dav Clark
layout: page
comments: true
---
{% include orgs.md %}

**Presenters can indicate their free times at [this poll](http://doodle.com/zkbndtimykd3g59v)**

## Course Description

This course addresses the fast-growing area of social and environmental
measurement using technologies such as mobile devices, “Internet of Things” (or
“Web of Things”) style sensors, and remote sensing. We will take a project-based
approach, with a classroom discussion each week, followed by a tutorial /
practicum in the [Berkeley Institute for Data Science][BIDS. Note that the focus
of this course is on data collection and management. Teams will likely do some
basic visualization and exploratory data analysis; statistics and/or machine
learning are not expected.  We will leverage support from the [Social Science
Matrix][Matrix], the [D-Lab][Dlab], [BIDS][BIDS], and [Berkeley Research
Computing][BRC] to provide necessary training, hardware, and compute resources.
This course is being offered as a part of the [BIDS Collaborative][DSC].

Students will work with project clients, who will help determine the project
roadmap. Note that the primary goal of the course is educational -- solving the
client challenges is a vehicle for learning. Credit will only be available to
individuals who are selected for project teams (ideal teams will include a
balance of individuals with project management, technical, and domain-specific
skills). The course will be open to drop-in attendance for all members of the
campus community.

Students should either know how to do basic scientific computing or be prepared
to learn outside of class (potentially with help from your classmates). In
addition, each week will only provide an *orientation* to the necessary skills
-- we can't provide an in-depth introduction to all of these topics in one
semester! Students will likely need to do additional learning to develop
meaningful skills.  Available resources on campus (e.g., in [D-Lab][Dlab] and
[BIDS][BIDS]) will be advertised to course participants.

## Planned classes

<ul class="post-list list-unstyled">

    {% for post in site.categories.syllabus reversed %}

        <li>
            <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} 
                {% if post.presenters %}
                    – {{ post.presenters }}
                {% endif %}
            </span>
            <h2>
                <a class="post-link"
                   href="{{ post.url | prepend: site.baseurl }}">
                     {{ post.title }}
                </a>
            </h2>
        </li>
    {% endfor %}

</ul>

## Aspirational Curriculum - Subject to change!

Please note, the curriculum is very much a work in progress.

 - Week 1
    - Lecture: Overview of issues in social and environmental measurement
    - Selection of team leads for projects
    - Practical: project management with GitHub, part 1
 - Week 2
    - Lecture: An introduction to ethical and legal concerns
    - Final selection of teams, codes available for telebears
    - Practical: Creation of team repositories, wiki, and project roadmap in
      issue tracker. Identification of needed technical resources, including
      budget.
 - Weeks 3-6 and 9-11 (order determined by plans from week 2 and speaker
   availability)
    - Intro to Jekyll / GitHub pages.
    - Basic data management (ODK Aggregate, Data Turbine, Postgres, MongoDB,
      ASbase)
    - Basic visualization (High-level d3, pointers to R and Python on your own)
    - Mobile devices (ODK, Data Turbine)
    - IoT/WoT sensors (Arduino + Bluetooth LE)
    - Remote sensing and geospatial data (Ecoengine, mapbox/leaflet, Google
      earth engine)
    - Administrative and utility data (Satellite imagery, Call record data,
      Electricity & Water)

 - Mid-semester (2 weeks)
    - Presentations: discuss successes, plans, and difficulties. Mid-semester
      presentations have a "technical" focus, with a goal of enabling your
      classmates.
    - Practical: teams and mentors work together to ensure successes are
      reproducible, pull in outside skills to address challenges. Videos of
      presentations reviewed by presenters and viewers.
 - Final presentations (2 weeks)
   - Discuss results in a non-technical fashion.
   - Practical: Finalize reproducible and transparent research reports (test
     reproducibility via other teams attempts to reproduce).

## Grading

Students enrolled in the class will get an A if they do all of the following, a
B if they partially complete at least all 3 items, and an incomplete otherwise.
This is meant to be a *very light* burden:

 1. Take notes or collect followup notes for at least one class,
 2. Make some progress on a project, document this, share it with another team,
    and incorporate feedback, and
 3. Provide such feedback to another team

Pre-requesite to the above are participation in the basic class systems
organized around GitHub. At a minimum, you will need to have a GitHub account
that gets associated with the class website and join our Gitter chat forum to
communicate with the class.

A general rubric for providing feedback is as follows:

 - Clarity / reproducibility of methods and results (presented on GitHub,
   assessed twice at mid-semester and final, strongly weighted towards final).
 - Quality of presentations (incorporating self assessment and peer assessment)
 - Quality of self assessment
 - Quality of peer assessment

Open questions:

 - Should all team-members get the same grade for team project? Or should teams
   be allowed to assign credit to different members?
 - How do students get credit for helping other teams?
