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

0. The first step of the process is to create a new example repository in GitHub. For these purposes you will need a GitHub account. If you don't already have a GitHub account please create one on [GitHub](https://github.com/) by following the steps outlined in the [official GitHub guide](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github).

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
> ```
"title": "My Title!",
"authors": [
    { "name": "Author1" },
    { "name": "Author2" }
]
```
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

6. According to the RSMD guidelines, the root of the repo should contain a citations file so that the software can be cited properly
    - to create a citation file in another browser tab, navigate to [https://citation-file-format.github.io/](https://citation-file-format.github.io/)
        - this is a tool that helps you develop citation files in the cff file format
    - click on Create CFF file in the upper right corner
    - click on the cffinit website blue button
    - choose Create
    - follow the workflow and define the content of citation.cff
    - download the file
    - drag and drop the citation.cff file in the root of your GitHub repo
    - discuss the data duplication in codemeta.json and citation.cff

7. Describe the research software in the README file using best practices
    - in a new browser tab navigate to [https://readme.so/editor](https://readme.so/editor)
    - create the content of the readme file using the sections templates provided
        - note that you are able to edit the content of one section at a time, but the preview on the right shows you the whole content of the readme file
    - download the completed readme
    - drag and drop the readme.md file in the root of your GitHub repo
    - once you commit the changes it will replace the old file

8. How you would publish the software once you are all done?
    - Zenodo provides a bridge with GitHub that simplifies the publication of your research software
        - for these purposes you first need to link your Zenodo account with your GitHub account
        - go to [https://zenodo.org/account/settings/linkedaccounts/](https://zenodo.org/account/settings/linkedaccounts/) and add GitHub
    - go to [https://zenodo.org/account/settings/github/](https://zenodo.org/account/settings/github/) and analyse the steps needed for publishing to Zenodo 
    - you must have noticed that one of the steps is to create a release on GitHub
        - you can try and create a release on GitHub (but don't link the repo on Zenodo so as not to create false records)
        - note that you should use semantic versioning for your releases
        - as this is your first release you should use the tag v1.0.0
        - provide release information and click on release
        - discuss what are the steps that need to be taken once you have obtained the DOI from Zenodo (is it just the readme file that needs to be updated?)

9. The last step is to create a record on Software Heritage to ensure your software is archived
    - in a new browser tab go to [https://www.softwareheritage.org/](https://www.softwareheritage.org/)
    - if this is your first time on this site then spend some time browsing around
    - to create a new record choose: Save Research Software
    - analyse the steps and check if anything is missing
        - if you have followed the steps above, then the AUTHORS file is still missing and needs to be added
            - to create an AUTHORS file, create a new file using a basic text editor
            - copy/paste the content of the example file from [Google Open Source](https://opensource.google/documentation/reference/releasing/authors)
            - make the necessary changes
                - to provide additional information on author roles take a look at [https://sdruskat.net/software-authorship/](https://sdruskat.net/software-authorship/) 
            - save the file as AUTHORS or AUTHORS.txt
            - drag and drop the file to the root of your GitHub repo
            - commit your changes
    - visit [https://archive.softwareheritage.org/save/](https://archive.softwareheritage.org/save/)
        - check if you are able to find the origin URL of your GitHub repo
        - do not submit so as not to create false records

10. If you still have time available you can now try and assess the FAIRness of your effort
    - for these purposes go to the FAIR assessment activity    

11. Prepare for retrospective
    - what are your main impressions of this activities in 2-3 sentences
    - choose a group representatives that will share these impressions with the rest of the workshop participants


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
Kjorveziroski, V., Filiposka, S. WebAssembly as an Enabler for Next Generation Serverless Computing. J Grid Computing 21, 34 (2023). [https://doi.org/10.1007/s10723-023-09669-8](https://doi.org/10.1007/s10723-023-09669-8)

The work is done as part of the OSCAR-2023 project, funded by FINKI-UKIM

## Summary

The steps outlined in this activity have aimed to guide you through the basic steps of the process of describing your research software with metadata. These are the essential steps that need to be done in order to improve the FAIRness of your software. The RSMD guidelines include additional information that has not been covered in this activity, but is also considered as very important when it comes to producing FAIR research software.

## Suggested Reading

- [D4.4 - Guidelines for recommended metadata standard for research software within EOSC](https://zenodo.org/records/8199104)
- [Create a CodeMeta file](https://codemeta.github.io/create/)
- [CodeMeta Governance](https://codemeta.github.io/governance/)
- [README.so](https://readme.so/)
- [CITATION file format](https://citation-file-format.github.io/)
- [Software Heritage](https://www.softwareheritage.org/)

