---
title: "Metadata for research software"
author: "FAIR-IMPACT"
tags: 
    - FAIR Software Objects
    - metadata
---

> the content of this page is based on [D4.4 - Guidelines for recommended metadata standard for research software within EOSC](https://zenodo.org/records/8199104) by FAIR-IMPACT

# Introduction

The FAIR-IMPACT Guidelines for recommended metadata standards for research software within the EOSC present the first proposal of the Research Software MetaData (RSMD) Guidelines, developed by Task 4.3 (T4.3), Standard metadata for research software, as part of Work Package 4, Metadata and ontologies, in the FAIR-IMPACT project. FAIR-IMPACT aims to realize a FAIR (Findable, Accessible, Interoperable, and Reusable) European Open Science Cloud (EOSC) by leveraging community guidelines and existing infrastructures in the scholarly ecosystem.

The growing recognition of software's crucial role in research has led to initiatives, infrastructures and research institutions to address the challenges of software findability, accessibility, attribution and reuse. One of these initiatives, the Scholarly Infrastructures for Research Software (SIRS) Task Force (TF), identified in its report (EOSC Executive Board & EOSC Secretariat, 2020) the general need for actionable, standardized guidelines for researchers/developers that self-archive software or submit software for publication.

The FAIR-IMPACT project acknowledged the rising need for establishing software metadata guidelines to effectively collect and curate metadata. In response, T4.3’s deliverable provides a comprehensive set of Research Software MetaData (RSMD) Guidelines that offer flexible and adaptable recommendations for end-users that can be used in different disciplines and different software development contexts.

This deliverable summarizes a large review and analysis including: a thorough introduction of the goals, methodology and use cases; the state of the art of existing practices and guidelines and the metadata landscape. Following the first introduction and state of the art, T4.3 introduces the RSMD guidelines proposal to collect and curate research software metadata. These guidelines are directly addressed to end users, including software creators and curators in their quest to improve the FAIRness of their software.

Lastly, T4.3 will continue its efforts to make the RSMD guidelines normative within the academic community. This includes engaging with stakeholders, gathering feedback, and incorporating best practices and advancements in metadata management within existing infrastructures. By establishing these guidelines as a norm, the aim is to promote widespread adoption and adherence, leading to greater standardization and harmonization of metadata practices across research domains. The ongoing commitment of T4.3 to refining and promoting the RSMD guidelines will contribute to the overall advancement of open and FAIR research practices in the research software community. The purpose of this deliverable in general and of the RSMD guidelines in particular is to provide a concrete and practical resource to support researchers in their endeavors to share and publish their research software creations.

## Describing and sharing software

The Scholarly Infrastructure for Research Software (SIRS) report (EOSC Executive Board & EOSC Secretariat, 2020) identified four major challenges that need to be addressed as ARDC:

- A for Archiving to ensure availability and accessibility
- R for Referencing to ensure precise identification for reuse and reproducibility
- D for Describing to ensure software can be found and understood
- C for Crediting to ensure proper acknowledgement of contributions and authorship

To establish a FAIR EOSC, software should be part of this goal following the high level FAIR for Research Software (FAIR4RS) principles specified in (Chue Hong et al., 2022) where artifacts should be at least findable, accessible, interoperable, and reusable (FAIR).

## Scope

FAIR-IMPACT uses the Research Software definition from the FAIR4RS output:

> Research Software includes source code files, algorithms, scripts, computational workflows and executables that were created during the research process or for a research purpose. Software components (e.g., operating systems, libraries, dependencies, packages, scripts, etc.) that are used for research but were not created during or specifically for research should be considered software in research and not Research Software. This differentiation may vary between disciplines. The minimal requirement for achieving computational reproducibility is that all the computational components (Research Software, software used in research, and hardware) used during the research are identified, described, and made accessible to the extent that is possible.
(Gruenpeter et al., 2021)

## Goals

FAIR-IMPACT Guidelines for recommended metadata standards for research software within the EOSC aim to: 

1. create a cohesive and standardized approach to research software metadata collection and curation that benefits all stakeholders involved; 
2. help the target audience identifying key requirements and best practices that can improve the quality and reproducibility of their research software.

## State of The Art of Best Practices and Guidelines

FAIR-IMPACT covers the main themes that are part of the prominent practices and guidelines both within and outside academia. The analysis is divided thematically, covering:

- Software development platforms and version control systems
- Accessibility and preservation (A = Archive)
- Reference and identification (R = Reference)
- Reuse, licensing and legal aspects
- Description and classification (D = Describe)
- Credit and attribution (C = Cite)
- Re-executability: dependencies and execution environment

## Metadata Analysis

FAIR-IMPACT explores and analyzes the roles and types of metadata in software collection, curation, preservation, and usage, distinguishing between intrinsic and extrinsic metadata.

Intrinsic and extrinsic metadata is defined as follows:

- Intrinsic metadata - Refers to the information that is inherently embedded within a software source code artifact. It includes metadata files that are captured in the main source code directory (such as README file, codemeta.json file, etc.)
- Extrinsic metadata - Refers to the information that is external to the software source code artifact. It includes metadata elements that provide context, provenance, and additional information about the software.

## RSMD Guidelines

The RSMD guidelines are a cross-disciplinary community driven effort to provide standardized and actionable guidance for the metadata collection and curation of research software. With the increasing importance of research software in academic research, it is necessary to ensure that software is archived, referenced, described and cited (ARDC) and that its metadata is findable, accessible, interoperable, and reusable (FAIR). The RSMD guidelines provide a framework for achieving these goals and facilitating the quality and sustainability of research software. Additionally, the guidelines can help stakeholders in the research community, such as researchers, software developers, research institutions, publishers, and infrastructure managers, identify requirements and best practices that are useful for their software.

The RSMD guidelines are organized into seven distinct aspects, each with a clear high-level objective and a set of actionable and detailed recommendations.

1. General Metadata Recommendations - To ensure the collection, curation, and maintenance of research software metadata, the following general recommendations are suggested for end users, including researchers, software engineers, curators, and institution staff.
2. Accessibility and preservation - To ensure accessibility and preservation, researchers and software engineers are strongly recommended to follow the archival and sharing recommendations below.
3. Reference and identification - To ensure that research software projects, modules, versions and source code artifacts can be precisely identified and referenced.
4. Description & classification - To ensure software findability and comprehensibility, provide descriptive metadata (software's name, purpose, functionalities, programming language, domain, etc.). These metadata facilitate accurate representation of the software and enable users to easily discover and understand its capabilities.
5. Credit & attribution - To ensure proper crediting and acknowledgment of software creators, authors, and contributors, it is important to follow citation recommendations.
6. Reuse, licensing and legal aspects - To ensure proper software reuse and license compliance, it is essential to accurately describe software licensing and legal aspects. This includes providing clear guidance on proper usage and distribution rights, clarifying the terms and conditions under which the software can be used and shared.
7. Re-execute: dependencies and execution environment - To ensure the usability of software and the ability to reproduce the same results in experiments, it is important that the software can be easily rebuilt and executed. This ensures that others can use the software effectively and achieve consistent outcomes.

## Making it Possible

FAIR-IMPACY has collected actions and requirements that should be executed by scholarly infrastructures (e.g scholarly repositories, aggregators and publishers) using the RSMD thematics, note that this list isn’t exhaustive:

- General requirements:
    - Ensure metadata records are licensed under CC0
    - Provide mechanisms to moderate and curate metadata to ensure curation quality of software records in the infrastructure collection
    - Provide specific guidance on how to use the infrastructure services to ensure metadata is collected and preserved 
- Accessibility & preservation:
    - Follow scholarly best practices identified by the scicodes consortium44 to ensure quality service, this includes but is not limited to: Providing a public scope statement, disclosing infrastructure end-of-life policy and stipulating conditions of use
- Reference and identification:
    - Provide tools to track the software in other scholarly outputs: aggregating information about entities and the relationships between them enables strategic analysis (Fenner, 2020)
    - Publish policies for research products including PIDs for software
    - Provide guidance to article authors to identify which PID should be used to identify software projects or artifacts: extrinsic and intrinsic identifiers
    - Implement platforms and services with better and consistent PID integrations and help grow the PID Graph to track connections.
    - Cross-link a plurality of academic outputs at the infrastructure level by providing adapted metadata properties
 - Description & classification
    - Share the metadata schema, taxonomy, vocabulary or ontology used by the infrastructure to store the metadata
    - Provide import and export metadata features using the codemeta.json format
- Attribution & credit
    - Provide citation export formats to facilitate credit (e.g BibTeX export format)
    - Establish clear authorship policy acceptable by the infrastructure (most relevant to publishers)
    - Provide mechanisms to cite collective author
- Reuse, licensing and legal aspects:
    - Provide standardized method for display copyright and licensing information between projects and people; e.g.: SPDX licenses list
    - Require license information using a controlled list (SPDX licenses list)
    - Support software authors by providing guidance on license use, etc.
- Re-execute: dependencies and execution environment
    - Provide metadata properties to store information about operating system, hardware and dependencies
    - Provide guidance, if possible, on how to ensure better sustainability of dull software stack (e.g GUIX)

## Summary

These guidelines focus on end-users, including researchers, software creators, and curators, during the process of collecting, curating, and managing software metadata. However, they are also applicable to various stakeholders, such as infrastructures that offer the required platforms, services, and tools to adhere to these guidelines.

Recognizing the significance of research software, these guidelines provide comprehensive recommendations for the collection and curation of metadata. They address challenges related to archiving, referencing, describing, and citing software, as well as guidance for ensuring the findability, accessibility, interoperability, and reusability of software within the scholarly ecosystem. The ultimate goal of these guidelines is to establish a FAIR EOSC that treats software on an equal footing with publications and data.



## Suggested Reading

- [D4.4 - Guidelines for recommended metadata standard for research software within EOSC](https://zenodo.org/records/8199104)

