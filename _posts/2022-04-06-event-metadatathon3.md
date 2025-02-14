---
layout: post
title: "AncientMetagenomeDir Metadatathon Apr. 2022"
categories: Events
sidebar_link: true
---

<img src="https://spaam-community.github.io/AncientMetagenomeDir/assets/images/spaam-AncientMetagenomeDir_socialmedia.png" style="display:block;margin-left:auto;margin-right:auto;width=50%;" width="50%">

## About

<!-- TOC depthfrom:2 -->

- [About](#about)
- [Organisational Details](#organisational-details)
  - [Who](#who)
  - [Where](#where)
  - [When](#when)
  - [What](#what)
- [Prerequisites](#prerequisites)

<!-- /TOC -->

It's time for AncientMetagenomeDir to level-up! Currently metadata about published ancient metagenomic samples stored at a sample level. However, for researchers working in the field, to maximise the utility of the resource we need to get closer to the data we actually use in our day-to-day work. For this, we need to expand to library and sequencing metadata, and start building an ecosystem to utilise the metadata itself.

As we are already utilising standardised _sample_ accession codes of data uploaded to public databases, we can already get a lot of this information automatically from the databases themselves, however some of this needs cleaning up, and there are some other bits of metadata that maybe useful not included in such repositories.
jeky
This event will consist of different components:

- **Training** on how to use Git(Hub), and AncientMetagenomeDir
- **Contributing** cleaned metadata and 'filling in the blanks' of all current sample-level metadata publications, as well as reviewing each other's contributions
- **Creating** a toolkit to allow efficient filtering and downloading of sequencing data based on filtering keywords based on the repository
- **Socialising**; getting to know each other, by having an informal environment allowing everyone to meet and chat about anything and everything

If we have sufficient progress, we aim to write a small paper introducing the toolkit. If you contribute metadata and/or code, you will be included as a co-author on the publication.

## Organisational Details

### Who

Anyone and everyone, from across the world! Both newcomers and veterans!

We are looking for as much help as possible, so if you have time (even for a couple of hours), it would be gratefully welcomed.

The more people we have, the better the workload distribution there will be for everyone.

### Where

We will be meeting on [gather.town](https://app.gather.town/app/gKwKhnaPw4B88ar7/spaam-community)! To learn how the platform works, please see the documentation [here](https://support.gather.town/help/movement-and-basics)

### When

- Date: April 6th 2022
- Time:
  - Due to the (aspired) global nature of SPAAM, we will be running this over multiple timezones:
    - Asia-Pacific
    - Europe, Middle East, & Africa
    - Americas

(All times following times are based on CEST, please see [this page](https://www.timeanddate.com/worldclock/converter.html?iso=20220406T070000&p1=47&p2=329&p3=313&p4=2010&p5=1306&p6=1376&p7=3336&p8=198&p9=24) for conversion to various cities)

| Date   | Time      | Event                                                               |
| ------ | --------- | ------------------------------------------------------------------- |
| Apr. 5 | 09:00 CET | **Group Check-in (Asia-Pacific): Welcome and training** (18:00 AUS) |
| Apr. 5 | <...> CET | Metadata processing and programming!                                |
| Apr. 5 | <...>     | Continue...                                                         |
| Apr. 6 | 09:00 CET | **Check-in/out (EMEA/Asia-Pacific): Welcome and training**          |
| Apr. 6 | 10:00 CET | Continue...                                                         |
| Apr. 6 | 11:00 CET | Continue...                                                         |
| Apr. 6 | 12:00 CET | **Lunch break (EMEA)**                                              |
| Apr. 6 | 13:00 CET | Metadata processing and programming!                                |
| Apr. 6 | 14:00 CET | **Check-in (Americas): Welcome and training**                       |
| Apr. 6 | 15:00 CET | Metadata processing and programming!                                |
| Apr. 6 | 16:00 CET | Continue...                                                         |
| Apr. 6 | 17:00 CET | **Check-out (EMEA)**                                                |
| Apr. 6 | 18:00 CET | Metadata processing and programming!                                |
| Apr. 6 | 19:00 CET | Continue...                                                         |
| Apr. 6 | 20:00 CET | Continue...                                                         |
| Apr. 6 | 21:00 CET | **Check-out (Americas)**                                            |

### What

The main bulk of the event consist of:

- Training on how to use Git(Hub) & the AncientMetagenomeDir structure (see [below](#prerequisites) if you want to practise beforehand!)
- Assigning yourself a publication & making a pull requests of:
  - Copied and pasting columns from an already generated (partial) library metadata table
  - Filling in columns that are not represented in the automated metadata table
  - Checking for accuracy of the columns
- Reviewing PRs to double-check accuracy

In addition, and in parallel, there will be a small team of software developers:

- Making a command-line tool to download and verify raw FASTQ files based on user-given filters
- Combine the new functionality with the current AncientMetagenomeDirCheck tool
- Extend the types of validation that be performed by AncientMetagenomeDirCheck
- (Stretch) auto-generate input table files for downstream tools

## Prerequisites

- Be interested in Ancient Metagenomics!
- Join the [SPAAM slack channel](../../home.md)!
- Register for a GitHub account and join the SPAAM-Community organisation (message James on Slack or send an [email](mailto:jfy133@gmail.com))
- Make sure you can access journal articles (institutional VPN etc.)
- Familiarise yourself with the ENA and/or SRA library browsers,
  - e.g. ENA: [https://www.ebi.ac.uk/ena/browser/view/PRJEB34569](https://www.ebi.ac.uk/ena/browser/view/PRJEB34569)
  - e.g. SRA: [https://www.ncbi.nlm.nih.gov/Traces/study/?query_key=1&WebEnv=MCID_6172841ce8ac3a04ad3ec535&o=acc_s%3Aa](https://www.ncbi.nlm.nih.gov/Traces/study/?query_key=1&WebEnv=MCID_6172841ce8ac3a04ad3ec535&o=acc_s%3Aa)
- Read through current AncientMetagenomeDir Guides for _sample_ metadata
  - [Adding a publication's _sample_ metadata](<https://github.com/SPAAM-community/AncientMetagenomeDir/wiki/Adding-a-Publication:-Step-by-Step-Guide-(Samples)>)
  - [Reviewing an AncientMetagenomeDir Pull Request](https://github.com/SPAAM-community/AncientMetagenomeDir/wiki/Reviewing-a-Pull-Request:-Step-by-Step)
