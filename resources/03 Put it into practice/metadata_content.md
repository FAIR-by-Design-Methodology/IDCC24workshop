---
title: "FAIR research software"
author: "Skills4EOSC & FAIR-IMPACT"
tags: 
    - FAIR-by-Design
    - FAIR Software Objects
    - Metadata for research software
---

# Introduction

The purpose of this activity is to learn the basics of following the RSMD guidelines and try out the main themes related to RSMD:

- Software development platforms and version control systems
- Accessibility and preservation (A = Archive)
- Reference and identification (R = Reference)
- Reuse, licensing and legal aspects
- Description and classification (D = Describe)
- Credit and attribution (C = Cite)
- Re-executability: dependencies and execution environment

by creating and describing an example repository of research software on GitHub.

## Learning Objectives

- describe research software using metdata
- publish research software on Zenodo
- archive research software on Software Heritage 

## Target Audience

- research software developers

## Duration

- 1 hrs

## Prerequisites

- familiarity with RSMD guidelines
- GitHub profile

## Learning Tools

- browser, online tools
- available example source code

## Describing research software using metadata

For the purposes of practicing the implementation of the RSMD guidelines we are going to create an example test source code repository on GitHub and describe the example software provided. Then we will take a look at the steps required to publish the repository on Zenodo and obtain a DOI and archive the repository in Software Heritage. We are not going to do any actual publishing or archiving to avoid adding test examples in the official catalogues.

Note: the steps in this activity are designed so that you don't need to have GitDesktop or any similar solution installed on your laptop to complete them. If you are familiar with using GitDesktop, you should make all changes to the repo using push and commit via GitDesktop

0. The first step of the process is to create a new example repository in GitHub. For these purposes you will need a GitHub account. If you don't already have a GitHub account please create one on https://github.com/ by following the steps outlined in the [official GitHub guide](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github).

1. Once you login to GitHub, you can create a new test repository by clicking on the New green button in the upper left corner.

2. Follow the steps of creating a repository
    - define the name of the repository
    - make the repository private, as we are creating a repository for learning and testing (otherwise it should be public)
    - choose Add a README file so that we can provide description of the repo
    - you don't have to add .gitignore at this point
    - choose a license (remember that in many situations your institution has a policy defining under license your research software should be available to others)
    - finally click on Create repository
    - the new repo will be created with two files inside: README.md and LICENSE

3. Add example source code to your repo (you can choose your own source code, or use the provided example)
    - we have prepared an example Jupyter notebook to serve as the source code together with some sample data
    - consider yourselves as authors and contributors for this example software
    - download the notebook and data sample from [Google Drive](https://drive.google.com/drive/folders/1JU7duwCmjianPiWO-iJ_0EcFAC5O9HHv?usp=sharing)
        - following best practices for repo structure there are two folders
            - src that contains an example Jupyter notebook that is our source code
            - samples that contains data samples that are the input for the notebook
    - unzip the downloaded file
    - drag and drop the two folders (src and samples) into your newly created repo
    - wait for the upload to be complete
    - change the commit message and description if you want 
    - leave the option to commit to main branch
    - click on Commit changes
    - you will then see both folders as part of your new repo

4. Add metadata to the Jupyter notebook
    - every Jupyter notebook has a metadata section where you can add your own metadata
    - go to the [JupyterLite demo page](https://jupyter.org/try-jupyter/lab/)
    - upload the test.ipynb file
    - open the test.ipynb file
    - in the menu go to view -> property inspector
    - in the advanced tools section on the right hand side you can now see the cell metadata and under the Notebook metadata
    - the new metadata should be added at the end of the Notebook metadata
    - add information about the title and authors by adding json code such as
> "title": "My Title!",
"authors": [
  { "name": "Author1" },
  { "name": "Author2" }
]
    - if you are not familiar with json, take a look at [this guide](https://stackoverflow.com/questions/66929384/add-notebook-author-and-title-in-jupyter-notebook-cells) on how to do it
    - save the notebook
    - right click on the notebook name and download the new version
    - navigate to the src folder on GitHub
    - choose add files in the upper right corner
    - drag and drop the new version of test.ipynb
    - commit the new change

5. Create a CodeMeta file to describe the research software
    - in a new browser tab go to [Create a CodeMeta file](https://codemeta.github.io/create/)
    - follow the link to the [CodeMeta Generator](https://codemeta.github.io/codemeta-generator/)
    - fill out the information 
        - to help you fill out some of the information in this form take a look at the brief description of the example software below
        - if some information is missing, take a look at the related paper, or simply invent it
        - discuss the unique identifier, how would you get one and when you are able to add this information
    - generate the codemeta.json
    - validate the codemeta.json
    - go back to your GitHub repo and create a new file
    - name the file codemeta.json
    - copy/paste the content from the generated file to the file on GitHub
    - choose commit changes in the upper right corner
    - codemeta.json should now be part of your repo

5. 




Describe the research software in the README file using best practices
    - 

Adapt file headers with info
Define Citation (citation.cff)
Define License 
Define Readme
Description
Dependencies
Test
…
Use SWH or Zenodo?
Review template for possible automated workflow
Measure the FAIRness of your effort
Paper based + 
Example tools that are in their development stage


### Brief description of the software

The Jupyter Notebook reads in measurements obtained using the hey benchmark and provides basic statistical information about the user response time under different conditions (type of application, type of deployment, type of infrastructure, number of requests per second, number of threads). The statistical information is saved in a csv format.

Language used: Python
Tested with Python v3.8.18 in Jupyter Notebook v6.5.4 using Anaconda 2.5.2 on Mac Sonoma 14.2.1.
Known dependencies: 

- Python 3
- Pandas
- matplotlib
- Seaborn
- pathlib

This notebook has been used to generate the results for the following paper:
Kjorveziroski, V., Filiposka, S. WebAssembly as an Enabler for Next Generation Serverless Computing. J Grid Computing 21, 34 (2023). https://doi.org/10.1007/s10723-023-09669-8

The work is done as part of the OSCAR-2023 project, funded by FINKI-UKIM

## Summary

At the end provide a short summary of the main points of the learning unit (these are the key takeaways that help reflect on the learning outcomes)

## Suggested Reading

- provide a list of references for further reading that should help clarify the content of the learning unit and elevate the knowledge level
- [Markdown guide](https://www.markdownguide.org/), free and open-source reference guide that explains how to use Markdown.
- [Create a CodeMeta file](https://codemeta.github.io/create/)
- [CodeMeta Governance](https://codemeta.github.io/governance/)

