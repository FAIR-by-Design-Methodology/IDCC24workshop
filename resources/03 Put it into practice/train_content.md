---
title: "FAIR learning materials"
author: "Skills4EOSC & FAIR-IMPACT"
tags: 
    - FAIR-by-Design Learning Materials
    - FAIR Learning Objects
    - FAIR assessment
---

# Introduction

The aim of this activity is to show case some of the elements necessary to develop FAIR learning materials. The main focus of the activity is on the definition of the logical organisation of the learning materials and all of their elements, both, learner facing and trainer facing as well as the definition of the main metadata for the learning materials.

## Learning Objectives

- analyse the FAIR-by-Design templates for learning materials
- use the RDA metadata schema for learning resources
- discover the trainer and learner content that should be defined for each learning unit
- assess level of FAIRness of learning materials

## Target Audience

- instructional designers, trainers

## Duration

- 1 hr

## Prerequisites

- familiarity with the FAIR-by-Design methodology stages
- nice to have: familiarity with MD and CFF formats

## Learning Tools

- browser, online tools (HedgeDoc, CFFINIT)

# Discover the elements of FAIR-by-Design learning materials

Although the FAIR-by-Design methodology in general does not define concrete formats, tools or methods for its implementation, for the purposes of development of learning materials within the Skills4EOSC project, we have developed a template repository on GitHub that can be used as a blueprint for the development of FAIR learning materials.  

Follow the defined steps to go through the activity and learn how to implement FAIR learning materials in practice using the templates repo as a blueprint.

1. Review the structure of the templates repo
    - the templates repository on GitHub can be found at [https://github.com/FAIR-by-Design-Methodology/templates](https://github.com/FAIR-by-Design-Methodology/templates)
    - go to the link and analyse the file structure
        - you can navigate to any file in the tree structure and preview the file content by clicking on the file
    - view the content of the following files:
        - README
        - LICENSE
        - CODE_OF_CONDUCT
        - CITATION
        - syllabus
        - template_facilitator_guide
        - training_feedback_template
    - analyse the structure of the Learning Unit folder
        - view the content of the learning content in template_content file
        - view the content of the information for trainers, (together with the facilitator guide and feedback they are known as the instructor kit):
            - template_unit_lesson_plan
            - activity_details_template
            - assessment_template
            - quiz_gift_template
    - Note: if you want to use this template repository as the starting point for your FAIR learning materials development you can follow the steps described in the Train the Trainers GitBook starting from [First Steps with Git](https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/Stage%204%20%E2%80%93%20Produce/08-Development%20Tools/08-Introduction%20to%20Markdown%20and%20Git/#activity-first-steps-with-git)

2. Analyse the content of an example Learning Unit
    - navigate to [https://github.com/FAIR-by-Design-Methodology/FAIR-by-Design_ToT](https://github.com/FAIR-by-Design-Methodology/FAIR-by-Design_ToT)
    - this repository holds all learning materials related to the Train the Trainers training for the FAIR-by-Design Methodology
    - the learners view of this repo content in the form of a GitBook is available at [https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/](https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/)
    - review the syllabus of the training which is the landing page of the GitBook
    - on GitHub, navigate into one example learning unit by your choice
    - make a comparison of what the learner can see, and what is the complete content of the learning unit
        - learning content
        - lesson plan
        - activities description
        - assessment
    - discuss the need for this additional files and why they should be available to trainers and other designers in editable format

2. Create your own syllabus
    - in the templates GitHub repository from step 1 navigate to the [syllabus file](https://github.com/FAIR-by-Design-Methodology/templates/blob/main/resources/syllabus.md)
    - change from preview to code 
    - copy the whole content of the file
    - in another browser tab, navigate to [https://hedgedoc.org/](https://hedgedoc.org/)
    - choose Try the demo, then Continue to demo instance
    - in the upper right corner choose + New guest note
    - paste the copied content in the editor window
        - note that the starting portion of the file between the two --- lines is the file header, this is where the machine-readable metadata is located
        - everything bellow the second --- line is the actual content of the file that is rendered and visible on the right hand side
    - provide human-readable metadata for your example training starting from Title of training (row 31 in the editor)
        - use the [Bloom's taxonomy](https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/Stage%201%20%E2%80%93%20Prepare/02-Preparing%20FAIR%20Learning%20Objects/02-Preparing%20FAIR%20Learning%20Objects_cont/#defining-learning-objectives) to define tangible learning objectives
    - provide machine-readable metadata in the file header
        - note that the content is the same, so you should be copy pasting information from below. The field names used in this part correspond to the names provided in the RDA minimal metadata schema
    - do you feel that the syllabus content is complete? taking into account the rest of the information that will be provided in each learning unit, is something missing in the syllabus?
    - note: you can download and save your effort by using the Menu in the upper right corner

4. Create your own citation file
    - unlike code_of_conduct where the only information required is an email address, or license where the file content is provided by CC, the citation file is a specific file wherein you need to provide the correct information so that it can be correctly processed
    - in the templates GitHub repository from step 1 navigate to the [citation file](https://github.com/FAIR-by-Design-Methodology/templates/blob/main/CITATION.cff)
    - copy the whole content of the file
    - in another browser tab, navigate to [https://citation-file-format.github.io/](https://citation-file-format.github.io/) 
        - this is a tool that helps you develop citation files in the cff file format
    - click on Create CFF file in the upper right corner
    - click on the cffinit website blue button
    - choose Update
    - paste the content of the copied citation file from the templates repo
    - click parse
        - there are two warnings as doi and license are not defined as basic fields, but the bottom message should say parsed CFF successfully
    - click start editing
    - note that this tool makes you choose between type of work software or dataset. As the learning materials are neither we recommend that the type field is not used in the file.
    - follow the workflow and define the content of citation.cff
    - ensure the file is valid
    - you can download the file for future reference
    - note that the citation file format provided in the templates repo is such that it is compatible with Zenodo
    - discuss if there is an automated way to avoid the need to enter duplicate information twice (compare citation and syllabus information)

4. Apply the QA checklist
    - within Skills4EOSC we have also developed a QA checklist that measures the level of FAIRness of the developed learning materials
    - in a new browser tab navigate to [FAIR-by-Design Methodology QA checklist](https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/Stage%206%20%E2%80%93%20Verify/19-Final%20QA%20check/19-finalQA/#fair-by-design-methodology-qa-checklist)
    - analyse the table and pay attention to the essential elements
        - if the learning materials lack an essential element that means that they are not complying with the minimum FAIR requirements
    - check the level of FAIRness of a chosen set of learning materials
        - does the material pass the minimum requirements?
        - if yes what is the total score obtained (X out of Y) if every question in the table weighs 1 point (notice that in some rows there are multiple questions) 

5. Prepare for retrospective
    - what are your main impressions of this activities in 2-3 sentences
    - choose a group representatives that will share these impressions with the rest of the workshop participants


## Summary

If you enjoyed the activity and would like to learn more about how to develop FAIR learning materials using the FAIR-by-Design methodology take a look at the training GitBook or simply enroll in the training course on the Skills4EOSC platform. The links are provided in the suggested reading list.

## Suggested Reading

- [FAIR-by-Design Learning Materials Methodology Training of Trainers on GitHub](https://github.com/FAIR-by-Design-Methodology/FAIR-by-Design_ToT)
- [FAIR-by-Design Learning Materials Methodology Training of Trainers GitBook](https://fair-by-design-methodology.github.io/FAIR-by-Design_ToT/latest/)
- [FAIR-by-Design Learning Materials Methodology Templates Repository](https://github.com/FAIR-by-Design-Methodology/templates)
- [FAIR-by-Design Learning Materials Methodology Training of Trainers on Skills4EOSC Learning Platform](https://learning.skills4eosc.eu/course/view.php?id=19)

