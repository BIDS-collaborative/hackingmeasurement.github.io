---
title: "BIDS, Moorea and Crete"
author: Dav Clark
layout: meeting
---

## In attendance

### Group from Crete

Neil met these folks at [JGI](http://usermeeting.jgi.doe.gov/).

 - Georgos - Marine population genetics, looking into microbial genomics
 - Evangelos - Bioinformatician, text mining for species names & descriptors,
   global collaboration for marine microbial sampling.
 - Eleni Hatziyanni - Government of Crete, resource management and planning

### BIDS

 - Karthik - Terrestrial Ecology, rOpenSci
 - Neil Davies - Moorea IDEA, Gump Field Station
 - Charlotte Cabasse - Ethnography
 - Dav Clark - D-Lab, Data Science Collaborative
 - Falk Schuetzenmeister - GIF, CNR, ecoengine

### Other Moorea/biocode folks

 - Jorrit Poelen - GLOBI, etc.
 - Maggie Kelly - ESPM & GIF, mapping
 - Suzi Lewis - LBL (selewis@lbl.gov)
 - Chris Mungall - LBL

## The story so far...

Started with genetic sequencing (biocode), expanding to bio-social understanding
throughout time:

 - How do we best represent that system today?
 - How did that system come to be in the past?
    - Geologically?
    - Ecologically?
    - Socially / human?
 - Simulate future states of the system.

Theoretical physicist from Switzerland (???)
Rich Williams, set up computational ecology group at MS Research, Cambridge.

Pilot project on water models.

20 "nodes" - organizational [clusters of people](http://mooreaidea.org/participants).

## On Crete

Realizing the value of good data encoding standards, data exchange and openness.

Setting up platform for data management, incorporating historical collections,
building capacity that could be applied to Moorea IDEA. Already working with
multiple communities.

Georgos has government research institute intended to be a hub for Greece on
bioinformatics, has a slide deck he uses to inspire traditional researchers to
join with the larger project. (Can we get a copy of these? Perhaps they'll need
translation.) This center is the largest in Greece, even larger than biomedical
research centers.

Crete is ~600,000 people in "23 Mooreas" in area. Also much less isolated system
than Moorea. E.g., economic crisis impacts the ecology of villages as young
people come back from cities. More specifically, there is a shift to organic
farming. In the north of Greece, it gets quite cold - folks cut down forests
illegally.

Charlotte is interested in the political transformation of Crete. What kinds of
political experiments can we observe (or perhaps support).

## What is the data science side?

Open science project. Are there ways Crete would like to contribute to Moorea
(or the IDEA infrastructure more generally)? Is there a community of "early
adopters?" What is central organization? Is there a technical framework (or a
social one)?

A core is available on **biocoding**, but Neil suggests this can be improved.
**Foodwebs** are similarly developed, still lots of data science challenges.

Stay focused on local, but want tools to be generally useful. Synthesis of data
from different projects is an ideal. This already happens in food web research
(genetic data, occurrence data, interaction occurrence, spatio-temporal, lots of
siloed research).

Jorrit suggests that we should start with making things useful, then proceed to
standards.

Karthik points out that things like this happen at LTER and pisco (sp?), but
very siloed. Data ONE has lots of funding, but it's all behind the scenes. Lean
approach could provide tools as they come to allow immediate leverage.

(Cross-referencing, this is somewhat different than what's currently happening
with ODK. It would be good to see what Matt, Waylon and crew think about the
dangers here - folks expect support once things are delivered.)

Concerns - BIDS can't do much beyond space and connections. We need funds to pay
a fraction of a person's time.

Talking about what BIDS can do - we should fly Tony Fountain up for a talk!

Pilot projects - folks have started building a 4D avatar presented on wall in
Zurich, ability to layer data (done by folks in Zurich, also working on
Singapore).

A central concern from Neil, keep physical model (for example) interacting with
social and biological models to avoid re-creation of scientific silos.

What is an avatar? Best representation of the thing (but there are many). Avatar
itself is not visible (it's too complex, humans can't see all of it).

Jorrit raises idea of two kinds of outputs - rough educational / public-facing
materials are easy, but still force debugging and integration of information.
Scientific applications can build on this effort to do more rigorous work.

Charlotte's question about how to use this for climate change education /
policy. Dav's response is that this is too hard, just make something interesting
that helps people explore according to their interest. Neil confirms this idea.

Evangelos has example of conveying messages with materials from human anatomy
textbooks?

### Specific proposals

 - Show top (marine) predators in Moorea ecosystem & what they rely on
   (including abiotic structures, water temperature...). Do the humans.
    - Coastal SEES - looking at coral reefs & fisheries
    - Coupled natural-human systems (has food webs)
    - Crete has many raptors, vultures, etc.
 - Commercial fish species (similar to above)
 - Mosquitos & infectious disease (for terrestrial)
    - Different mosquitos have different infectiousness (could perhaps even
      simulate with trait data)
    - Could tie into Crete with other vector studies?
 - Water? From different perspectives (i.e., species, geology)?
 - Simulate removal of marine protected areas / increase fisheries (reef turns
   to algae due to loss of herbivorous fish).

Relatedly - what makes its way to textbooks, and what remains only with experts?
There are very few complete food webs (most complete appear to be lake systems,
or marine).

We'd like an "ecologically aware" Google search. This is an extension of what
Tony Dell and colleagues did with their "One Cubic Foot" project. Example of
unjustified conflation between two types of hawkfish. Perhaps could have been
prevented with trait bank (e.g., mouth morphology) - work by Chris Meyer (has
data on what was in guts, biocoded these contents, then screened against
reference database).

 - Get interactions between software projects (e.g., EOL, GBIF, GLoBI). This
   would be available, e.g., in the references tab in GLoBI. Show interactions
   across tools, databases, primary literature, etc. Also show where things are,
   as a reference tool.

### Getting concrete

Can we get text mining data from Evangelos into GLoBI? Extend EOL? But his
system works better with sequences due to use of NCBI taxonomy. If want species
name without knowing exact DNA / ID, that could be a draft approach. This would
be a data source in the GLoBI ecosystem. Note that all species from Moorea will
have a sequence in the gene bank!

Hackathon in ID Bio (in Gainesville, FL) in June or so, looking at doing the
above.

Process of annotation of papers might be quite similar to Nick Anderson /
Hypothes.is / Text Threshr approach to news articles. Note funding from Sloan. Hybrid
approaches may help streamline this approach. Talk to Spencer about using this
tool?

Chris Mungall knows of literature on text mining protein-protein interactions.

BioHeritage library may be a good source.

GLoBI has a nice API where a group of students recently built a [species
interaction exploration tool](http://danielabar.github.io/globi-proto). You
could start [here](http://www.globalbioticinteractions.org/). Pictures coming in
via iNaturalist (curated by EOL).

## Needs

 - Tech
    - Compute?
    - Storage?
 - People
    - Programmers
    - Designers
    - Writers
 - Community
    - Conference (might include biology, and social science funding - Perhaps
      Matrix for both funding and / or space?)
