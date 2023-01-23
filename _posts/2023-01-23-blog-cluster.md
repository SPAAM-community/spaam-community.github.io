---
title: "Don’t get flustered! What’s a cluster? The use of the word 'cluster' in palaeogenomics"
date: 2021-09-13
authors:
  - James A. Fellows Yates
  - Åshild J. Vågene
tags: spaam, blog
---

## Don’t get flustered! What’s a cluster? The use of the word 'cluster' in palaeogenomics

## Introduction

_by [James A. Fellows Yates](http://jafy.eu/) and [Åshild J. Vågene](https://twitter.com/AshAshild)_

If you have ever listened to a talk in palaeogenomics, you may have noticed that the term 'cluster' is used a lot (or maybe you will after reading this post 😉).

This word is actually used in many different contexts with quite different meanings. Here we briefly introduce some of the variety of ways this term is commonly used in the field, to help you have a better idea what different people may be referring to in different contexts.

## **Illumina sequencing** _clustering_

In Illumina's [fluorescence-based](https://en.wikipedia.org/wiki/Illumina_dye_sequencing) sequencing, DNA molecules are immobilised on a glass slide to ensure they have a fixed position during imaging. This ensures the imaging camera can associate the light emission from each fluorophore to the corresponding DNA molecule.

However, the coloured light emission of a single fluorophore is not enough for the camera to pick up. Therefore, once immobilised, multiple copies of the DNA is made in this exact location using bridge amplification.

In the context of sequencing, **clustering** is the process of making lots of copies of the immobilised DNA molecule.

A **sequencing cluster** (the noun this time!) is the result of the Illumina sequencing clustering _process_. This is a single location on a sequencing flowcell containing many copies of a single DNA molecule.

On older models of Illumina sequencing machines, these clusters would be randomly distributed across a flowcell. However newer machines use 'patterned flowcells' that have a honeycomb-like regular distribution of surface depressions to ensure consistency of where sequencing clusters are generated, during the clustering process. 

In most cases you will not encounter these in your research unless you take on tasks as a sequencing technician, and in some very early stages of quality control such as "Per Tile Sequence Quality" sections of [FastQC results](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/3%20Analysis%20Modules/12%20Per%20Tile%20Sequence%20Quality.html).

## A **computing** cluster

A **computing cluster** is a [network of multiple servers](https://en.wikipedia.org/wiki/Computer_cluster) (called nodes), which allow high performance computing. These nodes are often linked by a central 'head-node' that all computing nodes are attached to - forming a 'cluster' around the head-node.

You will often use such clusters as offered by your institute to analyse your data.

Typically, you log-in to the head-node, and submit your analysis commands to a 'scheduler' on the head-node, which then uses algorithms to distribute the commands of all the users of the cluster across all the computing nodes in a computationally resource-efficient manner.

## A cluster **factor**

You  are most likely to encounter the term **cluster factor**, sometimes referred to as duplication factor, while using the ancient DNA pipeline [EAGER](https://eager.readthedocs.io/en/latest/index.html), [nf-core/eager](https://nf-co.re/eager), and/or the deduplication tool [DeDup](https://github.com/apeltzer/DeDup).

This term is a metric used to describe the number of PCR duplicates you have in a Next Generation Sequencing library; something that measures the concept of library 'complexity' or 'duplication'.

During library amplification or clustering, you end up with identical copies of the same original molecule that will also be sequenced. These duplicates are not that useful as they do not provide new or extra information over the original molecule. Such duplicates can cause artefacts in downstream analysis because they can result in over-inflated confidence, in that you may think that the "duplicate" molecule represents a second but identical molecule from the sample itself, while it actually just means that the same molecule from the sample got copied a few times (i.e. an artefact of PCR). Therefore researchers typically try to remove these duplicates _in silico_.

Researchers aim to have low duplication rates (also termed 'high complexity'), which suggests the DNA library has enough unique molecules to keep sequencing for more and more extra information. Users of the tools mentioned above ([EAGER](https://eager.readthedocs.io/en/latest/index.html), [nf-core/eager](https://nf-co.re/eager), and [DeDup](https://github.com/apeltzer/DeDup)) therefore use the **cluster factor** to decide whether it is worth sequencing further for higher coverage (and thus high confidence in downstream analysis).

The **Cluster factor** is calculated as the ratio of mapped reads before duplicate removal divided by mapped reads after duplicate removal. If you have a _low_ cluster factor (i.e. close to one), you could reasonably assume you will obtain more unique molecules by deeper sequencing of your library. If you have a _high_ cluster factor (e.g. >2), you generally would not want to sequence the library more, as you would not get more information, and therefore would not be cost-effective.

In ancient metagenomics, you will often see this in genomic analysis of microbes (such as in pathogen genomics), when sequenced library reads are aligned against the reference genome of interest. Researchers then perform deduplication prior variant calling to ensure confidence that the variant called is correct. If they may wish to sequence more, they would the check the cluster factor value to make this decision.

Note this is a rule-of-thumb metric, and for more accurate estimates of further sequencing effort you can use tools such as [Preseq](http://smithlabresearch.org/software/preseq/).

## A PCA cluster

Principal Component Analysis is an analysis technique that takes data with many different dimensions (read: relationships), and reduces these complex relationships in a way that can be displayed in just two dimensions. This is typically plotted in a 2-axes scatter plot.

A **PCA cluster** is an informal term to describe a collection of points that fall close together in a group on the scatter plot, and indicate some form of relationship compared to other points falling on a PCA.

In ancient microbiome analysis you can often see this method being used when performing authentication that your samples are well-preserved based on taxonomic profiles. A researcher could use PCA to see if their samples cluster with other well-preserved samples of the same type and fall away from other sample types that would indicate bad preservation (e.g. a soil control).

## Hierarchical clustering

**Hierarchical clustering** is another analytical method of finding relationships between different data, in the form of bifurcating tree-like patterns. This method tries to separate a set of samples (for example) into two groups (i.e., **clusters**), that are more similar to those within the same group than the samples in the other group. Each of these two groups can then further split into two smaller groups, again **clustering** samples by similarity, to produce four clusters. This procedure goes on and on until you have one 'cluster' per sample.

These are often displayed as trees, and associated with a heatmap to allow you to visualise why the clusters were formed based on the values of the multi-point dataset in the samples.

You will also often see this in ancient microbiome analysis when trying to find similarities and differences between the taxonomic profiles of different samples, with the associated heatmap representing the number of reads that aligned to each taxon in the taxonomic profile.

## Gene clustering

**Gene clustering** is used to describe the biological observation that two or more (sets of) genes of identical or similar sequences (e.g. ribosomal RNAs) cluster together on the same chromosome, or homologous chromosomes. This clustering implies that the sets of genes descended from one ancestral gene by duplication and diversification, groups of which are termed multigene families (e.g. human alpha and beta globin genes).

Gene clusters can vary in size from as few as eight genes (Hox genes) to two thousand (5S RNA on human chromosome 1).

## Summary

Overall, (palaeo)geneticists like to reuse the same fancy words to describe different things and this can often confuse newcomers to the field. We hope this post will help you navigate the minefield that can be scientific jargon.
