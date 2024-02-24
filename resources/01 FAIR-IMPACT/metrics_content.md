---
title: "FAIR Research Software Metrics"
author: "FAIR-IMPACT"
tags: 
    - FAIR Research Software
    - FAIR Assessment
---

> The content of this page is based on - [D5.2 - Metrics for automated FAIR software assessment in a disciplinary context](https://zenodo.org/records/10047401) by FAIR-IMPACT

# Slides

[Download the slides regarding FAIR Research Software Metrics here](https://github.com/FAIR-by-Design-Methodology/IDCC24workshop/raw/main/resources/01%20FAIR-IMPACT/FAIR%20Research%20Software%20Metrics.pptx){:download}


# Introduction

The deliverable from Task 5.2 (FAIR metrics for research software) on “Metrics for automated FAIR software assessment in a disciplinary context” is part of Work Package 5 on “Metrics, Certification and Guidelines“ within the FAIR-IMPACT project. It builds on the outputs of the RDA/ReSA/FORCE11 FAIR for Research Software WG and existing guidelines and metrics for research software to define metrics for the assessment of the “FAIR Principles for Research Software (FAIR4RS Principles)”. FAIR software can be defined as research software which adheres to these principles, and the extent to which a principle has been satisfied can be measured against the criteria in a metric. This work on software metrics was coordinated with Task 4.3 (Standard metadata for research software) from Work Package 4 on “Metadata and Ontologies”, which focuses on “Guidelines for recommended metadata standard for research software within EOSC“, to ensure that metrics are related to their recommended metadata properties.

The deliverable defines 17 metrics that can be used to automate the assessment of research software against the FAIR4RS Principles, and provides examples of how these might be implemented in one exemplar disciplinary context of the social sciences. The FAIR-IMPACT project will then work to implement the metrics as practical tests by extending existing assessment tools such as F-UJI; this work will be reported in Q2 2024. Feedback will be sought from the community, through webinars and an open request for comments. The information from all these sources will be used to publish a revised version of the metrics.

## Purpose and Scope

To increase the adoption and uptake of the FAIR principles, this deliverable presents 17 metrics that can be used to translate the FAIR guiding principles into practical tests to measure the FAIRness of research software, that can be implemented in an automated fashion via assessment tools for the different infrastructures in the scholarly ecosystem (software aggregators, software publishers, scholarly repositories and software archives).

The metrics are developed to be domain-agnostic, and take into account characteristics which are specific to research software such as its executability, its composite nature and its continuous evolution and versioning. Though most of the FAIR4RS Principles (summarised in Table 1) can be turned into a measurable metric, some (e.g. “F2. Software is described with rich metadata”) are much harder to quantify, and hence be assessed by any automated tool in the future. In these cases, it may only be possible to test for existence rather than quality or correctness. Others, such as “R3. Software meets domain-relevant community standards” can be seen to apply to many metrics, and the implementation of a metric will reference these community standards.

## FAIR4RS

The FAIR Principles for Research Software (FAIR4RS Principles) are (from Table 1 in Chue Hong et al., 2022):

F: Software, and its associated metadata, is easy for both humans and machines to find.

- F1. Software is assigned a globally unique and persistent identifier.
    - F1.1. Components of the software representing levels of granularity are assigned distinct identifiers.
    - F1.2. Different versions of the software are assigned distinct identifiers.
- F2. Software is described with rich metadata.
- F3. Metadata clearly and explicitly include the identifier of the software they describe. F4. Metadata are FAIR, searchable and indexable.

A: Software, and its metadata, is retrievable via standardized protocols.

- A1. Software is retrievable by its identifier using a standardized communications protocol.
    - A1.1. The protocol is open, free, and universally implementable.
    - A1.2. The protocol allows for an authentication and authorization procedure, where necessary.
- A2. Metadata are accessible, even when the software is no longer available.

I: Software interoperates with other software by exchanging data and/or metadata, and/or through interaction via application programming interfaces (APIs), described through standards.

- I1. Software reads, writes and exchanges data in a way that meets domain-relevant community standards. I2. Software includes qualified references to other objects.

R: Software is both usable (can be executed) and reusable (can be understood, modified, built upon, or incorporated into other software).

- R1. Software is described with a plurality of accurate and relevant attributes.
    - R1.1. Software is given a clear and accessible license.
    - R1.2. Software is associated with detailed provenance.
- R2. Software includes qualified references to other software. 
- R3. Software meets domain-relevant community standards.

## FAIR Metrics

The metrics presented in the next sections are specified following the template, modified from Wilkinson et al. (2018) and Devaraju et al. (2022):

- Metric Identifier - The local identifier of the metric (FRSM-XX) FRSM: FAIR Research Software Metric.
- Metric Name - Metric name in a human readable form.
- Description - The definition of the metric, including examples.
- FAIR4RS Principle - The FAIR4RS principle(s) most related to the metric.
- RSMD Recommendation - The FAIR-IMPACT RSMD recommendation(s) most related to the metric
- Assessment - Requirements and methods to perform the assessment against the metric. This includes a suggested compliance level (essential / important / useful), based on the concepts introduced by the FAIR Data Maturity Model Working Group (2020). Criteria at each level will change as adoption of FAIR increases.
- Comments - Further notes associated with the implementation of the metric, which may include related resources, constraints and limitations.

List of FAIR Research Software Metrics:

- FRSM-01 - Does the software have a globally unique and persistent identifier?
- FRSM-02 - Do the different components of the software have their own identifiers?
- FRSM-03 - Does each version of the software have a unique identifier?
- FRSM-04 - Does the software include descriptive metadata which helps define its purpose?
- FRSM-05 - Does the software include development metadata which helps define its status?
- FRSM-06 - Does the software include metadata about the contributors and their roles?
- FRSM-07 - Does the software metadata include the identifier for the software?
- FRSM-08 - Does the software have a publicly available, openly accessible and persistent metadata record?
- FRSM-09 - Is the software developed in a code repository / forge that uses standard communications protocols?
- FRSM-10 - Are the formats used by the data consumed or produced by the software open and a reference provided to the format?
- FRSM-11 - Does the software use open APIs that support machine-readable interface definition?
- FRSM-12 - Does the software provide references to other objects that support its use?
- FRSM-13 - Does the software describe what is required to use it?
- FRSM-14 - Does the software come with test cases to demonstrate it is working?
- FRSM-15 - Does the software source code include licensing information for the software and any bundled external software?
- FRSM-16 - Does the software metadata record include licensing information?
- FRSM-17 - Does the software include provenance information that describe the development of the software?

## Summary

The FAIR Impact project will work to implement the metrics as practical tests by extending existing assessment tools such as F-UJI; this work will be reported in Q2 2024.

## Suggested Reading

- [D5.2 - Metrics for automated FAIR software assessment in a disciplinary context](https://zenodo.org/records/10047401)

