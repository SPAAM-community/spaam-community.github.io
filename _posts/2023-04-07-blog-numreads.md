---
layout: post
title: "How deep do I screen? Read allocation when shotgun sequence screening for ancient pathogens"
date: 2023-04-07
categories: Blog
authors:
  - Kevin Daly
tags: spaam, blog
---

## How deep do I screen? Read allocation when shotgun sequence screening for ancient pathogens

_by [Kevin Daly](https://www.tcd.ie/Genetics/molpopgen/kevin_d.php)_


Hello everyone! My name is [Kevin Daly](https://www.tcd.ie/Genetics/molpopgen/kevin_d.php), I’m a post-doctoral researcher based in Trinity College Dublin, Ireland. This blog post is motivated by the beginnings of a project to search for ancient animal pathogens among some of the earliest livestock remains.

This is the first project which I’ve been involved in which explicitly hopes to identify pathogen DNA amongst endogenous host reads and exogenous environmental reads. Typically our group screens DNA from archaeological material using shotgun sequencing using an Illumina MiSeq (aiming to obtain 50,000 - 200,000 reads per sample) or an Illumina NovaSeq (aiming for 500,000 - a few million reads per sample) prior to deeper sequencing. While this is ample for host DNA identification, it may be insufficient to confidently find microbial DNA from ancient extractions which are known to contain DNA from many different sources. The literature suggests that pathogen DNA is often much less abundant than host or environmental DNA (although this will vary by sample, tissue type, pathogen identity etc);  it’s not uncommon for papers to report just a few dozen reads of pathogen origin during the screening stage.

We plan to generate and bioinformatically screen dozens of DNA libraries using [Kraken2](https://github.com/DerrickWood/kraken2) and other tools; missing true positive signals due to insufficient amount of screening reads would be a huge blunder. This motivated my question on the SPAAM “No-Stupid-Questions” channel and this blog post: “What is the (minimum) # of TOTAL reads people generally target for screening with the hope of picking up pathogens/specific microbes?”

Five million reads per sample was a recurrent answer as the typical amount of shotgun sequencing data per sample that could then be searched for pathogen DNA. [Gunnar Neumann](https://www.shh.mpg.de/person/94792/25522) (The Max Planck Institute of Geoanthropology, Germany), [Pooja Swali](https://www.crick.ac.uk/research/find-a-researcher/pooja-swali) (The Francis Crick Institute, UK) and [Åshild Vågene](https://globe.ku.dk/staff-list/?pure=en/persons/644451) (The Globe Institute, Denmark) all recommend at least 5 million reads per sample to detect pathogens or specific microbes. Pooja gave some additional perspective, warning that pathogens which cannot be detected among 5 million reads may be too difficult to work with further even after enrichment, due to poor coverage or ancient damage interfering with genome reconstruction. 

The genetic characteristics of the pathogen also influences screening decisions. For example, viral genomes are much smaller than bacterial ones and so require a greater amount of total sequencing to be detectable. As an aside, how preservation and degradation patterns of ancient pathogen DNA varies across pathogen type (i.e. bacteria vs viral; gram positive vs gram negative bacteria; different protein shells which encapsulate viral genomes, etc.) remains under-explored. [Meriam Guellil](https://www.heas.at/about/members/meriam-guellil/) (University of Vienna, Austria) warns that 5 million reads may not be sufficiently deep sequencing for viral reads to be detected. To paraphrase Åshild, if you are searching for samples containing ancient viral DNA, the more shotgun data the better! Similarly, libraries with a shorter overall fragment length profile will benefit from additional sequencing. However, the inherent challenge of identifying the origin of shorter DNA sequences will limit confidence in taxonomic or genome assignment. Libraries with median fragment lengths closer to the 30-35bp range - the typical (but not universal) minimum length cut-off - may require additional allocated reads to make confident taxonomic assignments.

Having access to more screening data proved to be useful for [Kelly Blevins](https://www.durham.ac.uk/staff/kelly-blevins/) (Durham University, UK), who generated between 8 - 10 million reads per sample in her search for pathogen DNA. Kelly then implemented competitive mapping and assessed breadth of coverage statistics to identify reads of *Mycobacterium tuberculosis* origin. However the spectre of randomness and low preservation (not unfamiliar to those working in ancient DNA) still looms. Kelly reports a library sequenced to a depth of 10 million total reads which was positive for *Treponema pallidum* DNA only contained 31/ 10,000,000 reads aligning to the *T. pallidum* genome. While it’s difficult to say if this particular sample is indeed positive for pathogen DNA, it would have undoubtedly been missed with less screening data.

A summarized answer from the SPAAM community is that typically 5 million reads is a reasonable minimum target for the confident identification of specific microbe DNA. However, there are many factors influencing the expected proportion of microbial DNA within an ancient DNA library: overall preservation, the amount of host and environmental DNA, the nature of the target genome, stochasticity. If additional sequencing capacity is available, aiming for ~10 million reads per library is strongly recommended. After surviving hundreds if not thousands of years, it would be a shame for these ancient disease agents to remain hidden, just shy of the detection threshold.  



---


*Editor’s Note: Do you, too, want to share questions and have a diverse range of ancient metagenomics researchers weigh in? Join our community at the [SPAAM Slack](https://join.slack.com/t/spaam-community/shared_invite/zt-1sm8wax7r-SbMYaFWSCC_CaTtNBzKwKw) where there are indeed no stupid questions! –Ele and Shreya*
