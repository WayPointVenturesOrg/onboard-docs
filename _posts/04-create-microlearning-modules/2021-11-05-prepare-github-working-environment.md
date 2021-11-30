---
layout: page
title: Prepare a working environment in GitHub
subtitle:
description: How to create a fork, the module scaffolding, and the MLS branch by working in GitHub and VSC
author: kcarlson
date: 07 Nov 2021
post-number: 4.5
category: create-microlearning-modules
position-in-category: 5
video_url: "none"
---

This page contains:

- Overview
- Install and set up Visual Studio code
- Create a new fork in GitHub
- Clone the fork in VSC
- Create scaffolding with VSC extension
- Create unit markdown files
- Fill in .yml metadata

## Overview

Toward the end of development, the MLS moves all the module content into a new fork in GitHub. Here's an overview of the steps. The MLS:

1. Installs and sets up Virtual Studio Code (VSC) on their computer.
1. Creates a copy (a *fork*) in GitHub of the existing GitHub Microsoft repository (*repo*).

    - The module content during development exists in this new MLS fork. 
    - The MLS doesn't ever merge this MLS fork back into the Waypoint/Microsoft fork. This is done by Microsoft after development and final sign-off.

1. Creates a copy (*clones*) the MLS fork, using VSC, to their own computer.
1. Creates the folder structure and files for all the files in the published module (called *scaffolding*) using a VSC extension.

1. Creates the unit markdown files using the text from the module doc and a program called Typora.
1. Fills in the additional information, or *metadata*, to files that were created automatically when the scaffolding was created.

    > **Tip:** The Module template has notes to guide the MLS when adding metadata to the .yml files.

## Install and set up Visual Studio Code

Visual Studio Code (VSC) is used to work with the module files.

- The module unit files are in a code language called *markdown*, which is similar to HTML. Markdown files have the .md extension. 
- The YAML files have the .yml extension. They are used in the published course to provide information about the course.
- Other files include images and graphics. These will have either a .png or .svg.

### What the MLS should install

The MLS should install:

- [Visual Studio Code](https://waypointventures.github.io/docs/install/install-vsc.html) to edit markdown and other module files. 
- [Docs Authoring Pack](https://waypointventures.github.io/docs/install/install-author-pack.html) to expand VSC with markdown-specific tools like a spell checker, markdown syntax, and the [Docs Scaffolding extension](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-scaffolding).
- [Word Count extension](https://waypointventures.github.io/docs/install/install-wordcount-ext.html) to display a word count in open markdown files.

## Create a new fork in GitHub

To create a fork (copy) of the repo in your GitHub account: 

1. In a browser, the MLS should log in to GitHub and then navigate to the Microsoft/Waypoint repo.

    > **Note:** As of this writing, to access the learn-pr code repo, the GitHub and v- accounts need to be linked. Refer to the instructions at [GitHub account setup](https://review.docs.microsoft.com/en-us/help/contribute/contribute-get-started-setup-github?branch=master).

1. Select the *Fork* button and then confirm your GitHub account as the location for the new fork.

![The Fork button in GitHub](../assets/images/github-create-fork.png)

## Clone the fork in VSC

After you create a fork of the repo, you'll be able to access and work on your fork from your computer using VSC. You do this by creating a local copy of the fork on your computer called a *clone*. You make changes to the clone (on your computer) and then periodically upload the changes to the fork in GitHub.

Select the **Clone** button. This copies the address of the repo into your clipboard. 

***graphic***

Switch to VSC on your computer.
Select **View** > **Command Pallette** > **Git: Clone**.
**Ctrl+V** to paste the address and then press Enter.

## Create scaffolding with VSC extension

To create scaffolding automatically, be sure the **Docs Authoring Pack for VS Code** extension for VSC is installed.
This extension includes the **Docs Scaffolding** extension which the MLS uses to auto-generate (*scaffold*) a skeleton module based on one of the standard module patterns:

- [Standard](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-standardmodules)
- [Introduction](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-intromodules)
- [Choose](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-choosemodules)
 
To create the scaffolding for a Standard Learn module:

1. In VSC, select the **Explorer** button. Navigate to the parent folder, in which you want to create the module folder.
1. Right-click the parent folder and choose ***Learn: Create module in CURRENT folder***.

    ![Create module in current folder option.](../assets/images/vsc-create-module-scaffolding-1.png)

1. Select **Standard**.

    ![Select the option for a Standard module.](../assets/images/vsc-create-module-scaffolding-2.png)

1. Enter the module name, all lower-case, using dashes to separate the words (not underscores), and then press Enter.

    ![Enter the module name.](../assets/images/vsc-create-module-scaffolding-3.png)

### What is created in the module scaffolding

A folder is created with the module name you specified. Inside the folder are sub-folders and files.

![Project scaffolding in VSC](../assets/images/vsc-create-unit-yml-files.png)

Inside the module folder are the following:

- An **includes** folder used to store the unit (markdown) files. In the includes folder, there are markdown files for each unit in the module.  The files contain template text help create the module content following Learn best practices. They are:
  - 1-introduction.md
  - 2-learning-content.md
    - Make a copy of this file for each learning content unit in the module.
  - 3-exercise.md
    - Remove if the module doesn't contain an exercise.
  > **Note:** Manually add a 4-knowledge-check.md file.
  - 5-summary.md
- A **media** folder used to store the module images and media files.
- The following YAML files (with a .yml extension):
  - 1-introduction.yml
  - 2-learning-content.yml
    - Make a copy of this file for each learning content unit in the module.
  - 3-exercise.yml
    - Remove if the module doesn't contain an exercise.
  - 4-knowledge-check.yml
  - 5-summary.yml
- index.yml file with the default metadata updated.

> For more detailed information, refer to [Create scaffolding](https://waypointventures.github.io/docs/add-content/scaffold.html) or [Create scaffold template](https://review.docs.microsoft.com/en-us/help/learn/create-scaffold-template?branch=main).








> For more detailed instructions, please refer to <a href="https://review.docs.microsoft.com/en-us/help/learn/create-scaffold-template?branch=main" target="_blank">Scaffold a module using the Docs Scaffolding extension for VS Code ![external link](../assets/images/extlink.png)</a>.










## Create unit files

Each unit in the module must have both a markdown (.md) and a YAML (.yml) file. The files should be numbered in the order they appear in the module.

The unit markdown files contain the content of the unit. The MLS adds this content from the Module Word document by using Typora. More detailed instructions for this process are in 

## Fill in metadata

The scaffolding YAML files contain placeholder text the MLS replaces with the real information from the Design or Module Word documents. Each YAML file also has one line that includes the file name for the associated markdown file.

> **Tip:** The Microlearning combined template.dotx file has comments to help the MLS move the information from the template to the YAML files.
 

## Update files in GitHub

After making changes to files in VSC, the MLS saves and uploads the changed files to GitHub. The first time this is done, VSC will prompt the MLS to create a Pull Request.

[Create a new branch in VSC](https://waypointventures.github.io/docs/branches/new-branch.html)
[Invite collaborator](https://waypointventures-my.sharepoint.com/personal/karinca_waypoint_ws/Documents/Invite collaborator)





Working with files in GitHub

There is a specific process to use to make changes in files in GitHub. 

Because multiple people will have access to the files, it’s crucial that you and your team communicate with each other about who should be editing files at any given time. Note: This is less of a concern if most of the development is done in Word. 

The most-recent files need to be copied to your computer in a process called *cloning.* You make changes in VSC Code to the local files (on your computer) and then copy them back to GitHub in a two-step process: commit and push. “Commit” saves your VSC changes to your local files. “Push” copies them back “up” to GitHub.

If you have a recent clone but you’re not sure if other people have made changes to the files since you worked on them last, you can use an “old” clone and do a “pull” before you start working. When you “pull” files, the latest files in GitHub are copied to your local files. Be aware that if you’ve made changes locally and haven’t pushed them up, doing a pull will write over your local files and you’ll lose your changes.

\1.   Get the most-recent files from GitHub: New clone or existing clone + pull 

\2.   Work in VSC Code and save your changes locally.

\3.   Move your changes back to GitHub: Commit and then push to your branch.

Note that when you clone, you are cloning from your branch, and from the root of your branch. You might need to “drill down” to the folder that contains your files.

Further reading

[Update branch (pull) in VSC](https://waypointventures.github.io/docs/branches/pull-updates.html)

[Send (push) files](https://waypointventures.github.io/docs/branches/push-files.html)

[GitHub/Azure DevOps development FAQ](https://waypointventures.github.io/docs/appendices/faq.html)

**More resources** 

 

Useful links (use your v- to access) 

·    [Learn Contributors Guide](https://review.docs.microsoft.com/learn-docs/docs/) – All the information that you ever wanted to know about what makes Learn content can be found here. 

·    [Docs Contributors Guide](https://review.docs.microsoft.com/help/contribute/) – Because Learn runs on Docs, our guidance is inclusive of this contributors guide as well. You'll find many cases where we default to the Docs guidance, so this is a great resource as well. 


·    [Microsoft Style Guide](https://styleguides.azurewebsites.net/StyleGuide/List) – Great place to reference if you're not sure on terminology. 

·    [learn-pr](https://github.com/MicrosoftDocs/learn-pr) – Here's where all of our content lives. 

·    [Microsoft Learn Azure DevOps](https://dev.azure.com/ceapex/Microsoft Learn/_backlogs/backlog/Waypoint/Stories/?showParents=true) – This is a backlog I created to track the work for this project. I'm in the process of adding all the members to the team, so this may not work for you at the moment, but should soon. 

·    [Instructional design home page](https://aka.ms/learn/id) – Use this resource to get information on our instructional design practices. 

·    [MS Learn & Waypoint Collaboration team](https://teams.microsoft.com/l/team/19%3a8859dd55812a40139162ac2a962100d9%40thread.tacv2/conversations?groupId=f2da37a2-23fa-4374-bae0-a0c08a9af078&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47) – Private team for our projects. Feel free to reach out here for anything specific to our project. 

·    [Microsoft Learn team](https://teams.microsoft.com/l/team/19%3ae71b47303a114990a3f0748661f48929%40thread.skype/conversations?groupId=2cd70980-6c76-45e6-8b88-02ea0b1fd561&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47) – This is an open team where anyone can post questions or get any information on Microsoft Learn in general. 

# YAML scaffolding 

Some of the content that students encounter is pulled from YAML files known as scaffolding or ‘work items’. 

The YAML files are created by Microsoft with several elements marked “to do,” that the MLS or SME needs to fill in. There are three types of files you will need to fill in: 

\1.    **Index (1 per module)**: The index file provides information about the overall module. Fields you need to fill in are: 

a.   Summary (maximum 35 words). [See How to write introductory summaries for modules and learning paths](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-introductory-summaries?branch=master). 

b.   Abstract (in this module, you will): fill in the learning objectives. Specifics are provided in the [Learning objectives section](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-learning-objectives) of the Learn documentation. 

c.   Prerequisites ([Prerequisites section](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-prerequisites)) 

\2.    **Unit files**: there is a file for each unit. Add a “short” summary and check that the time listed is accurate. The [scaffold manually section](https://review.docs.microsoft.com/en-us/learn-docs/docs/create-scaffold-manual) of the Learn documentation includes samples and explanations. The Learn documentation [How to write good meta descriptions](https://review.docs.microsoft.com/en-us/help/contribute/contribute-how-to-write-seo-meta-description?branch=master) provides more information and examples edited descriptions. 

·    **Current meta description:** Consume REST web services in Xamarin apps. (41 characters) 

- **Edited meta description**: In this learning module,     learn how to consume REST web services with HttpClient as part     of Xamarin applications. (111 characters) 

1. **Knowledge checks**: all questions and answers need to     be placed the YAML file structure. 

·    A knowledge check is a two to ten question assessment that measures if the learner has acquired the skills outlined in the learning objectives 

o  A Knowledge Check embedded in another unit file must have 2-3 questions 

o  A Knowledge Check as a standalone unit must have 3-5 questions. 

o  The module summary unit cannot contain a Knowledge Check. 

o  Every module must have at least one Knowledge Check unit – and it must be the penultimate unit in the module. 

·    Write questions that support learning 

o  Write questions as a complete sentence ending with a question mark 

o  All answers in a multiple-choice question should be about the same length, this avoids cueing the learner to select the longest or shortest answer in a group. 

o  Provide three plausible answers and don’t include “all of the above” or “none of the above” as a choice. 

o  Avoid using the words “not” and “except” in questions 

o  If the answers are numeric, list in sorted order. 

o  **Use third person, not “you”** 

o  **Avoid using fictitious people names in questions (raises bugs).** Instead, use a generic title, example, “an administrator”. 

·    Provide a meaningful explanation for both correct and incorrect answers, for example: 

o  More information is provided in the Learn documentation section [How to write knowledge checks](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-knowledge-check) 

 

**Markdown code sample to model** 

Most knowledge check information goes in the YAML file. For the Markdown file simply add the following. 

Choose the best response for each of the questions below. Then select “Check your answers.”  

**Knowledge checks in YAML** 

The code “scaffolding” is provided for you in the Knowledge Check YAML file in green text. You will need to add all ToDo as well as the questions and answers (true and false versions) as in the screenshot below. 

![img](file:///C:/Users/Karin/AppData/Local/Temp/msohtmlclip1/01/clip_image002.jpg)


