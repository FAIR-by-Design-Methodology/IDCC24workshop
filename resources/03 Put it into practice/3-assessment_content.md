---
title: "FAIR assessment"
author: "Skills4EOSC & FAIR-IMPACT"
tags: 
    - FAIR-by-Design
    - FAIR Software Objects
    - FAIR assessment
    - FAIR4RS
---

# FAIR assessment

FAIR software objects can be assessed for their level of "FAIRness" in order to ensure that all FAIR aspects have been successfully considered and implemented. Many of the [FAIR for Research Software Principles (FAIR4RS)](https://doi.org/10.15497/RDA00068)can be implemented by following the [Guidelines for recommended metadata standard for research software within EOSC](https://zenodo.org/doi/10.5281/zenodo.8097536), which provide a comprehensive set of Research Software MetaData (RSMD) Guidelines that offer flexible and adaptable recommendations for end-users. 

To perform FAIR assessment one can use a FAIR software checklist and manually go through it point by point. Another option, that FAIR-IMPACT and others are currently working on. is to use an automated tool to help in this process. 

## Learning Objectives

- understand the relationship between FAIR software metrics, research software metadata, and automated assessment
- assess the FAIRness of software objects

## Target Audience

- research software developers, research software engineers, librarians, curators

## Duration

- 1 hr

## Prerequisites

- familiarity with software source code repositories
- familiarity with FAIR principles
- familiarity with FAIR software metrics

## Learning Tools

- browser, online tools
- FAIR assessment checklist

## FAIR assessment of software objects

1. Choose a software repository to assess
   - If you already have your own software repositories where you have developed and kept your research software you can use it as the object for which you will assess its current level of FAIRness.
      - in case you are going to use your own, feel free to go quickly through the FAIR research software activity and add any missing metadata to your software
   - If not, then choose one of the following example software repositories to assess:
      - [F-UJI](https://github.com/pangaea-data-publisher/fuji)
      - [howfairis](https://github.com/fair-software/howfairis)
      - [isseven](https://github.com/meadsteve/isseven)

2. Use the FAIR software checklist developed by FAIR-IMPACT to assess the FAIRness of the chosen software object
    - analyse each item of the following table by paying attention to the requirements, method, essential, important and useful aspects
    - note that the specification for each of the metrics is available in [D5.2 - Metrics for automated FAIR software assessment in a disciplinary context](https://zenodo.org/records/10047401), chapter 2 Metric Specification page 12

| **Identifier** | **Name** |
|---|---|
| **FRSM-01** | Does the software have a globally unique and persistent identifier? |
| **FRSM-02** | Do the different components of the software have their own identifiers? |
| **FRSM-03** | Does each version of the software have a unique identifier? |
| **FRSM-04** | Does the software include descriptive metadata which helps define its purpose? |
| **FRSM-05** | Does the software include development metadata which helps define its status? |
| **FRSM-06** | Does the software include metadata about the contributors and their roles? |
| **FRSM-07** | Does the software metadata include the identifier for the software? |
| **FRSM-08** | Does the software have a publicly available, openly accessible and persistent metadata record? |
| **FRSM-09** | Is the software developed in a code repository / forge that uses standard communications protocols? |
| **FRSM-10** | Are the formats used by the data consumed or produced by the software open and a reference provided to the format? |
| **FRSM-11** | Does the software use open APIs that support machine-readable interface definition? |
| **FRSM-12** | Does the software provide references to other objects that support its use? |
| **FRSM-13** | Does the software describe what is required to use it? |
| **FRSM-14** | Does the software come with test cases to demonstrate it is working? |
| **FRSM-15** | Does the software source code include licensing information for the software and any bundled external software? |
| **FRSM-16** | Does the software metadata record include licensing information? |
| **FRSM-17** | Does the software include provenance information that describe the development of the software? |

3. Use an automated tool to assess the software FAIRness
    - Although there are FAIR assessment tools for data, few are currently available for assessing software. 
    - Some examples of FAIR assessment tools for software that you can try include:
       - [FAIR Software Checklist](https://fairsoftwarechecklist.net/): this is a web checklist that asks you 15 questions about your software. This is similar to the FAIR-IMPACT metrics.
       - F-UJI: web version designed for data, though can be used for software. A software specific set of metrics is being implemented.
       - howfairis: Python tool that needs to be installed on your computer. Doesn't directly assess against the FAIR for research software principles.

5. Compare the results from both approaches
    - discuss any problems or doubts during the process
    - what metrics did you find most useful to consider?
    - what metrics did you find hardest to check?
    - what metrics would you change to be more useful for your community / discipline?

6. Prepare for retrospective
    - what are your main impressions of this activities in 2-3 sentences
    - choose a group representatives that will share these impressions with the rest of the workshop participants


## Summary

By performing FAIR assessment of your research software you are able to pinpoint the problems and find guidelines that will help you overcome them making your solution more easily findable, accessible, interoperable and reusable.

## Suggested Reading

- [D5.2 - Metrics for automated FAIR software assessment in a disciplinary context](https://zenodo.org/records/10047401)

