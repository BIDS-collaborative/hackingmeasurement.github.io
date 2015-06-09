---
title: "BIDS, Moorea and Crete"
author: Dav Clark
layout: meeting
---
*May 16th, 2015 Additions: Evangelos Pafilis*

## In attendance

### Group from Crete

Neil met these folks at [JGI](http://usermeeting.jgi.doe.gov/).

 - [Georgos](http://www.imbbc.hcmr.gr/users/georgios-kotoulas) - Marine
   population genetics, looking into microbial genomics
 - [Evangelos](http://epafilis.info) - Bioinformatician, text mining for
   species names & descriptors, global collaboration for marine microbial
   sampling.
 - [Eleni
   Hatziyanni](https://www.linkedin.com/profile/view?id=196506212&trk=eml_inv_status_profile) -
   Government of Crete, resource management and planning

### BIDS

 - [Karthik - Terrestrial Ecology, rOpenSci](http://bids.berkeley.edu/people/karthik-ram)
 - [Neil Davies - Moorea IDEA, Gump Field Station](http://bids.berkeley.edu/people/neil-davies)
 - [Charlotte Cabasse - Ethnography](http://bids.berkeley.edu/people/charlotte-cabasse)
 - [Dav Clark - D-Lab, Data Science Collaborative](http://bids.berkeley.edu/people/dav-clark)
 - [Falk Schuetzenmeister - GIF, CNR, ecoengine](http://bids.berkeley.edu/people/falk-schuetzenmeister)

### Other Moorea/biocode folks

 - [Jorrit Poelen - GLOBI, etc.](https://www.linkedin.com/in/jhpoelen)
 - [Maggie Kelly - ESPM & GIF, mapping](http://bids.berkeley.edu/people/maggi-kelly)

### Berkeley Lab - Lewis Lab

 - http://www2.lbl.gov/lsd/People_&_Organization/Scientific_Staff_Directory/Lewis_Lab.html
 - http://berkeleybop.org/: Berkeley Bioinformatics Open-source Projects
 - [Suzi Lewis - LBL](http://berkeleybop.org/person/suzanna-lewis) (selewis@lbl.gov)
 - [Chris Mungall - LBL](http://berkeleybop.org/person/chris-mungall)

## The story so far...

Started with genetic sequencing (biocode), expanding to bio-social understanding
throughout time:

 - How do we best represent that system today?
 - How did that system come to be in the past?
    - Geologically?
    - Ecologically?
    - Socially / human?
 - Simulate future states of the system.

Theoretical physicist from Switzerland (Matthias Troyer (ETH) et al. ?),
Rich Williams, set up computational ecology group at MS Research, Cambridge.

- See: http://ogdoad.ethz.ch/idea/Home.html (1st Island Digital Ecosystem
  Avatars Workshop ETH Zürich, November 18 – 20, 2013) on “Grand Challenge
  Questions”
- See: Nature News: “Tropical paradise inspires virtual ecology lab”
  http://www.nature.com/polopoly_fs/1.16710!/menu/main/topColumns/topLeftColumn/pdf/517255a.pdf 
- See: http://mooreaidea.org/data for the different types of data being
  integrated: BIOCODE, CRIOBE, MCR LTER, MIRADA, Landscape model, Bathymetry,
  Social, Archeological

Pilot project on water models.

20 "nodes" - organizational [clusters of people](http://mooreaidea.org/participants).

## On Crete

Realizing the value of good data encoding standards, data exchange and openness.

Setting up platform for data management, incorporating historical collections,
building capacity that could be applied to Moorea IDEA. Already working with
multiple communities.

Georgos has government research institute intended to be a hub for Greece on
bioinformatics, has a slide deck he uses to inspire traditional researchers to
join with the larger project. This center is the largest in Greece, even larger
than biomedical research centers.

Crete is ~600,000 people in "23 Mooreas" in area. Also much less isolated system
than Moorea. E.g., economic crisis impacts the ecology of villages as young
people come back from cities. More specifically, there is a shift to organic
farming. In the north of Greece, it gets quite cold - folks cut down forests
illegally.

Charlotte is interested in the political transformation of Crete. What kinds of
political experiments can we observe (or perhaps support).

A hub for single-point-access to the Greek Biodiversity Data, Information and
Knowledge is being setup.  The relevant project is
"https://www.lifewatchgreece.eu/", the Greek node of the EU LifeWatch
infrastructure (http://lifewatch.eu).

## What is the data science side?

Open science project. Are there ways Crete would like to contribute to Moorea
(or the IDEA infrastructure more generally)? Is there a community of "early
adopters?" What is central organization? Is there a technical framework (or a
social one)?

A core is available on **biocoding**, but Neil suggests this can be improved.
**Foodwebs** are similarly developed, still lots of data science challenges.

see PDF: [Workshop: Food Webs for Model Islands Berkeley Institute for Data
Science, Berkeley, California, 27­28 April
2015](http://mooreaidea.org/storage/pdfs/moorea.foodweb.workshop.2015.pdf)

Stay focused on local, but want tools to be generally useful. Synthesis of data
from different projects is an ideal. This already happens in food web research
(genetic data, occurrence data, interaction occurrence, spatio-temporal, lots of
siloed research).

Jorrit suggests that we should start with making things useful, then proceed to
standards. Find 2, 3 use cases, list data scripts to be used (e.g. rOpenSci).

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

e.g see [the association of the kallikrein-related peptidase 3 (prostate
specific antigen) with different tissue types of the human
body](http://tissues.jensenlab.org/Entity?figures=tissues_body_human&knowledge=10&experiments=10&textmining=10&type1=9606&type2=-25&id1=ENSP00000314151)

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
    - Model and predict: if you reduce water how will it affect mosquito population?
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

 - Get interactions between software projects (e.g., EOL, GBIF, GLoBI,
   ENVIRONMENTS-EOL). This would be available, e.g., in the references tab in
   GLoBI. Show interactions across tools, databases, primary literature, etc.
   Also show where things are, as a reference tool.
 - ENVIRONMENTS and related projects:
   - ENVIRONMENTS: Identification of Environment Descriptive Terms in Text
     http://environments.hcmr.gr/
   - SPECIES and ORGANISMS: Identification of Taxonomic Mentions in Text
     http://species.hcmr.gr   
   - EXTRACT: Interactive Extraction of Environment Metadata
     http://environments.hcmr.gr/biocreative.html
   - [Cretan Bird - Environment distribution:
     visualization](http://environments.hcmr.gr/cretan-birds/summarize.html)
     This is merely a visual summary of the environments (ENVO terms mined from
     the EOL - “global scale”) for birds associated with Crete (according to
     GBIF occurrence data – “local scale”). Landscape ecology, citizen science
     and other projects could be supported from such integrative analysis. Data
     from the “global scale” could be used to make predictions at the “local
     scale”, e.g. “in which type of environment according to the global
     literature might a bird be found in unexplored region?”
 - “Polytraits: A database on biological traits of polychaetes”
   http://polytraits.lifewatchgreece.eu/ , a manually curated database on
   biological traits of polychaetes (bristle worms, Polychaeta: Annelida).
   - The list of the full trait definitions is available at:
     http://polytraits.lifewatchgreece.eu/terms 
   - “supporting evidence” is being tracked e.g. 
     http://polychaetes.lifewatchgreece.eu/taxonomy/term/5126/traits
     ![Larval development](/images/LarvalDevelopment.png)
   - please contact Dr. Faulwetter (sarifa@hcmr.gr) for more information

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

BiodiversityHeritageL library (http://www.biodiversitylibrary.org/) may be a
good source. BHL in collaboration with Prof. Ananiadou, Dr Navarro (NACTEM, UK)
and other colleagues are already working on  http://miningbiodiversity.org/

GLoBI has a nice API where a group of students recently built a [species
interaction exploration tool](http://danielabar.github.io/globi-proto). You
could start [here](http://www.globalbioticinteractions.org/). Pictures coming in
via iNaturalist (curated by EOL).

### More todo

"Guts of the Avatar" 

 - Paragraph for Phenotype RCN funding - working meeting modeling species
   interactions: ontologies and other data science approaches.

List from a few select data sources (papers, experts) from a few key (island) systems (Moorea/Crete/Hawaii) on terms they use:

 - Relationship types (slide from Chris Meyer; and from Evangelos)
 - Body part terms
 - Life history stages/states terms 
 - Basis of observation (evidence type) for interactions

Map those terms to ontologies

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
