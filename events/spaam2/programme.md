---
layout: page
title: SPAAM2 - Programme
---

### Session Structure

Length: 2 days

All times CEST (see here for Time Zone
[conversion](https://everytimezone.com/s/e15fccf5))

#### Day 1

- _13:00_ Welcome and Introductions
- _13:30_ **Session 1** [Trash in, trash out: Optimizing and standardizing
  laboratory practices in ancient metagenomics](#session-1)
- _15:00_ Break
- _15:15_ **Session 2** [Removing the persistent trash: Challenges in genotyping
  and filtering out contaminant reads from genome alignment](#session-2).
- _17:30_ Long Break
- _18:30_ **Session 3** [Sorting and Recycling the Trash: authentication,
  standards, and reproducibility in ancient metagenomic research (Part
  1)](#session-3).
- _20:00_ Daily Wrap up
- _20:15_ Finish

#### Day 2

- _13:00_ Day Overview
- _13:10_ **Session 4** [Sorting and Recycling the Trash: authentication,
  standards, and reproducibility in ancient metagenomic research (Part
  2)](#session-3).
- _15:30_ Break
- _15:45_ **Session 5** [Reuse the refuse: Applying new analytical methods
  beyond current practises](#session-5)
- _18:00_ Long Break
- _19:00_ **Session 6** [Discussion: Future steps for SPAAM](#session-6)
- _20:00_ Daily Wrap up
- _20:15_ Finish

### Abstracts

All sessions will include 'icebreaker' talks by members of the SPAAM community,
who will present on their own experiences and challenges working ancient
metagenomics to serve as starting point for discussions.

:warning: All titles and abstracts are subject to minor changes!

#### Session 1

**Title** Trash in, trash out: Optimizing and standardizing laboratory practices
in ancient metagenomics

**Chair** Irina Velsko

**Abstract** Optimizing laboratory practices is necessary to reduce the amount
of contaminating DNA in a sample extract, and subsequently in sequencing data.
All sequenced contaminating DNA takes up information that should be for sample
DNA, reducing the efficiency of workflows, both financially and
bioinformatically. Further, sample biomass influences the amount of "spill-over"
that is observed in sequence data, where the contents of higher biomass samples
may show up in lower biomass samples. In this session we will discuss how best
to prevent or reduce introduction of contamination to sample extraction and
library building protocols, as well as limiting sample cross-contamination.
These techniques aim to improve sequencing efficiency by reducing the amount of
sequenced contamination and increasing the amount of sequenced sample DNA.

**Icebreaker presenters** Jaelle Brealey and Zandra Fagernäs

**Icebreaker mini-abstract** _Reducing contamination: how to minimize the amount
of trash_ Contaminants can be introduced to samples during excavation,
post-excavation handling and storage and processing in the laboratory. Minor
differences between sample processing batches and cross-contamination between
samples processed together can also cause problems in downstream analyses. In
this talk we will discuss methods to reduce and control for external
contamination, batch effects and cross-contamination during laboratory
processing of ancient samples.

#### Session 2

**Title** Removing the persistent trash: Challenges in genotyping and filtering
out contaminant reads from genome alignments

**Chair** Åshild (Ash) Vågene

**Abstract** Genotyping is the characterization of variants (SNPs, Indels) that
occur at the single genome level. Accurate genotyping of ancient microbial
genomes is crucial for downstream analyses, such as phylogenetic placement, SNP
effect analysis and molecular dating. Genotyping is also important for taxonomic
profiling when trying to perform strain separation. Thus, inaccuracies in
genotyping/variant calling can have an enormous impact on the interpretation of
the results.

Confounding factors related to these genomes being a) ancient, b) from
metagenomic backgrounds, can negatively impact genotyping efforts by causing
multiallelic variant calls that infringe on thresholds for calling homozygous
variants. These factors include ancient DNA damage, short reads prone to
mis-mapping in regions of genomic rearrangement and cross-mapping of
contaminating sequences derived from genetically similar organisms from the
specimens’ burial/storage environment. Approaches such as edit distance and
analysing the allele frequency of multiallelic positions are commonly used to
give an indication of the level of ‘contamination’ in an alignment. Both
molecular and computational approaches exist to mitigate the effects of
contaminant and mis-mapping reads in genotype calling.

In this session we will discuss issues and problems relating to genotyping of
ancient microbial single-genomes, with emphasis on (but not restricted to)
haploid bacterial and viral genomes. The aim of the session is not only to make
others aware of specific issues/scenarios that may arise from working with
different types of microbes, but also to have a general discussion of the best
approaches to tackle such problems.

**Icebreaker presenters** Susanna Sabin and Kun Huang

**Icebreaker mini-abstract 1** _One man's trash..._ Though consensus sequences
are required for many valuable analyses, researchers in ancient DNA and
microbial genomics in general must also acknowledge that single consensus
sequences called from NGS data rarely reflect biological reality, even in clonal
organisms. If the aDNA community is able to methodologically and culturally step
outside the phylogenetics box, it could open the door to important, time
structured evolutionary insight we lose by not considering the true variation of
target organisms within our samples. The problem is, what is true variation in
an ancient metagenomic sample?

**Icebreaker mini-abstract 2** _Building consensus alleles with awareness of
position-specific damage probability_ To reconstruct the whole genome sequence
of ancient bacteria, many recent studies use alignment-based approach by 1)
aligning sequencing reads against a single reference sequence and 2) extracting
consensus base from aligned reads. However, this strategy is artefact-prone when
consensus site is decided by bases which are positioned on the ends of most
aligned ancient reads where post-mortem damages are frequently observed.
Therefore, we introduce a possible computational solution which could ameliorate
the quality of reconstructed ancient bacterial genomes by precisely removing
nucleotide bases of ancient reads which are possibly affected by post-mortem
damage.

#### Session 3

**Title** Sorting and Recyling the trash: Defining authentication guidelines for
the research community

**Chair** Clio Der Sarkissian and James Fellows Yates

**Abstract** Authenticating ancient metagenomic datasets has long been
considered equally a nearly impossible and crucial task to demonstrate that
‘true’ ancient metagenomes can be characterised. Post-mortem fragmentation
(typically via depurination) and damage base modification (via cytosine
deamination) make aDNA analysis very sensitive to exogenous ‘contaminating’ DNA
that can confound downstream analysis. Validation of results is therefore
imperative not only to ensure scientific rigour, trust in the methods by
researchers from related fields (e.g., anthropologists, archaeologists), but can
also have important ethical consequences. Defining a consensus-based legitimate
set of minimum-authentication criteria for ancient metagenomics is therefore
crucial for gaining this trust in the field and facilitating further exploration
of this type of data. Secondly, following standard guidelines by researchers can
only be expected if these standards and guidelines follow FAIR principles:
Finable, Accessible, Interoperable, and Reusable. Making sure authentication
methods and reporting guidelines can be used and applied by any type of lab (big
or small, specialist or generalist), can only come by making sure software and
data is accessible, usable and most importantly understandable. In part one of
this two-part session we will: i) get an overview of the obstacles and possible
solutions of current and potential future approaches for authenticating
metagenomic datasets, ii) begin to define a minimal authentication line of
evidence and iii) discuss how to communicate this to collaborators inside and
outside the ancient metagenomic community. In part two we will discuss i) how to
improve accessibility and usability of ancient metagenomic datasets and software
such as through collaboratively-generated benchmarking/comparative datasets as
well as metadata reporting, and ii) how to ensure responsible and ethical
research conduct.

**Icebreaker presenters** Sterling Wright, Nikolay Oskolkov, Nicolás Rascovan,
James Fellows Yates, and Miriam Bravo López

**Icebreaker 1 & 3 mini-abstract** _Improving current and future practices in
ancient microbiome analyses_ In this presentation, we will discuss the different
challenges in the bioinformatic processing and analysis of ancient microbiome
data. This includes: i) compiling reference datasets and comparative analyses,
ii) using standardized authentication tools, iii) identifying the limitations of
current methods and analysis strategies, iv) recognizing community needs and
designing more efficient methods, v) publishing studies that benchmark and
validate strategies, vi) establishing database creation and handling, and vii)
promoting open source and crowdsourcing initiatives. In particular, we will
review how all of these topics affect authentication tools implemented in
ancient microbiome studies, such as the commonly used SourceTracker. We hope
that an open discussion on these issues will serve as a guide towards towards
more robust and reproducible analysis in future research

**Icebreaker 2 mini-abstract** _Improving authentication tools of ancient
microbiomes_ In this presentation, I will discuss alternative ways of performing
authentication analysis in ancient metagenomics data. Specifically, with low
amounts of aDNA and a lack of good quality refernce genome, there is a need for
going beyond traditional alignment and deamination pattern approaches, when
addressing authenticity of each individual sequence. I will discuss how Machine
and Deep Learning algorithms could help to infer authenticity of individual
ancient metagenomics sequences in a reference genome free manner.

**Icebreaker 4 mini-abstract**: _Towards standards in metadata reporting in
ancient metagenomic studies: experiences from AncientMetagenomeDir_ One of
the first and last part of most ancient metagenomic studies is to gathering
or reporting basic metadata about samples and their sequences. A recent SPAAM
community project established AncientMetagenomeDir, a comprehensive but
lightwieght collection of lists of all published ancient metagenomic and
microbial genome samples. In this icebreaker I will cover the challenges
encountered during this data scraping exercise, and introduce one possible
proposal to improving metadata reporting in our field.

**Icebreaker 5 mini-abstract** _Ethics in ancient pathogen genomics_ The
emergence of biological and historical interpretations through ancient DNA
research, in particular through ancient pathogen genomics, can have important
social, legal, and political consequences for individuals and communities.
Therefore, the discussion of the best ethical practices within the field will
allow us to promote responsible research on ancient pathogen genomics.

#### Session 5

**Title** Reuse the Refuse: Applying new analytical methods beyond current
pratises

**Chair** Anna Fotakis and Alex Hübner

**Abstract** Throughout its history the field of ancient genomics has
traditionally been playing catch-up by creatively adapting the advances achieved
in modern genomics to their own types of datasets. Although this process has not
been without setbacks, it steadily pushed the field forward and allowed it to
apply the same methods as when using modern DNA. The newest technological
advancement that took over metagenomics is de-novo assembly, whereby short reads
from an environmental sample are assembled into novel microbial genomes. Its
application to sequencing data from present-day samples has led to a rush of
thousands of new metagenomic-assembled genomes (MAGs) from uncultivated
microorganisms and allowed scientists to investigate the “unknown” at large
scales for the first time. However, its application to sequencing data from
ancient samples has just started and still requires thorough evaluation and
fine-tuning of its parameters to make it suitable for this special type of
sequencing data. In this session, we want to discuss the challenges that come
along with applying de-novo assembly strategies to ancient metagenomic data and
highlight potential pitfalls in the current workflows. Furthermore, we want to
develop some guidelines on how to interpret this new type of results and
establish which conclusions can be drawn from them, in order to avoid
long-lasting mistakes that come along when adapting new methods to ancient
genomics. Finally we would like to encourage novel ways of approaching datasets
building upon previous sessions of SPAAM2 regarding public data sharing
deposition.

**Icebreaker presenters** Maxime Borry and Antonio Fernandez-Guerra

**Icebreaker mini-abstract 6**: _New take on ancient DNA metagenomics assembly
validation_  
Given enough sequencing depth, it is now possible to assemble ancient DNA data
into contigs using de novo assemblers. However, sorting the contigs originating
from modern contamination, from contigs assembled from truly ancient DNA, can
require a lot of manual work that does not scale easily with the immense number
of assembled contigs. With the Pydamage approach of damage estimation and
statistical testing, we show how to rapidly filter for contigs showing ancient
DNA damage, to be used for further analysis.

**Icebreaker mini-abstract 7** The adoption of modern metagenomic methods to
explore ancient metagenomes and gain insight into their functional potential are
starting to increase in their popularity amongst the community. However, we
should act with caution and be aware of their limitations. I will go over some
of the challenges of applying those approaches when analyzing ancient
metagenomes and provide some ideas for developing computational methods tailored
to our needs.

#### Session 6 - Future Steps for SPAAM

**Abstract** Now that we have identified common obstacles and discussed possible
solutions for our field, what's next? In this session we will summarise
everything talked about in the last two days. We can identify potential common
projects and 'working commitees' to begin work on these topics. Finally we will
gather opinions on future meet ups, e.g. a SPAAM3.
