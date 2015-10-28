---
title: Ecostations Data Access Monitor (EDAM)
client: Jorrit Poelen, EDAM
topic: Large-scale data integration, web-standards "database", and visualization
mentor:
team:
layout: project
---
## Project links

 - [EDAM GitHub repo](https://github.com/BIDS-collaborative/EDAM)
 - [EDAM on
   ![Gitter](https://badges.gitter.im/Join%20Chat.svg)
   ](https://gitter.im/BIDS-collaborative/EDAM)
 - [EDAM Static Demo](http://bids-collaborative.github.io/EDAM/)

## Progress Summary

We identified 4 islands - Moorea, Kauai, Friday Harbor (San Juan Island), and 
the Galapagos islands - to demonstrate the proejct idea. After reading an 
[article](http://www.nature.com/ncomms/2015/150907/ncomms9221/full/ncomms9221.html)
on biodiversity studies, we defined a metric for completeness and collected
biodiveristy data on birds regarding these islands. Using leaflet.js for maps,
we constructed a [simple tool](http://bids-collaborative.github.io/EDAM/) for
comparing the bird biodiversity among the islands. The tool is static, but it 
demonstrates the project's intent of allowing biodiversity analysis and comparisons 
to promote data sharing and research collaboration.

## Background

This will be phase 1 of a larger project to construct species lists, food webs
and associated citations.

As large biodiversity collections and environmental data are accessible online,
global research communities have an unprecedented access to (siloed) datasets.
Now that methods are within reach that allow to combine and process
biodiversity data at global scales, institutions can start to re-examine
existing data to coordinate data collection efforts, evolve data sharing
strategies and discover methods to efficiently sustain our (island) ecosystems.
A first step toward integrating the data is to provide a side-by-side
comparison of existing data associated with active island ecostation
communities to stimulate knowledge sharing and collaboration.

## Project Description

Ecostation biodiversity data summaries are derived from openly available
biodiversity data repositories (e.g. GBIF, iDigBio, GloBI). Initially only
species lists and associated food webs are compiled for participating
ecostations using automated data processing algorithms. For each ecostation,
the completeness of the lists and webs are estimated. Also, the similarity of
the lists and webs are calculated across the spatially separated island
ecosystems to highlight ecological likeliness.

By providing EDAM, spatially and institutionally disjoint projects now have a
data-driven method to see how much ecological data is available for specific
spatio-taxonomic spaces. We hope that comparing available ecological data
across ecostations will help stimulate collaboration between scientists,
technologists, educators, local governments and research foundations to help
better understand and sustain ecosystems around us.

In order to archieve EDAM Phase I, we need to:

 1. identify 3-5 island ecostations (e.g. Moorea/Oahu/Friday Harbor)
 2. define/identify spatial and taxonomic ranges for ecostations
 3. generate/retrieve spatio-taxonomic species checklist at scale and on-demand
    (e.g.https://github.com/jhpoelen/effechecka, Map of Life mol.org)
 4. construct local biotic interaction webs based on species interaction data
    and spatially explicit checklist: occurrence + interaction = local biotic
    interaction web estimate.
 5. develop/adopt similarity measures for checklists and biotic interaction
    webs
 6. develop/adopt completeness measures for checklists and biotic interaction
    webs
 7. create a visualization to make results (and associated data sources) easy
    to access.

## Contributors

name          | github handle    | nano-bio 
------------- | ---------------- | ---
Jorrit Poelen | @jhpoelen        | freelance software engineer building open tools for open data 
Jonathan Wang | @jonathanwang017 | junior studying CS / Stats 
Nisreen Hejab | @nhejab          | Ph.D student in Biophysics/Structural Biology
Carlo Liquido | @koalaboy808     | Graduate student in School of Information
Jong-kai Yang | @GitOnion        | Graduate student in School of Information
Vedant Saran  | @vedants         | Freshman studying EE/CS
Tong Zhang    | @tongzhang1995   |  
{: .table}


Given that the data is already available and the limited scope of needed data
processing capabilities, a first prototype of EDAM Phase I is estimated to take
2-3 months for a group of digitally literate graduate students with allocation
of ~10hrs a week. The outcome of this project will help define future funding
to further develop advanced phases of the EDAM project.
