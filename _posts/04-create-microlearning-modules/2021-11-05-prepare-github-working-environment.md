---
layout: page
title: Prepare VSC and GitHub
subtitle:
description: How to set up VSC and prepare a working environment in GitHub.
author: kcarlson
date: 07 Nov 2021
post-number: 4.5
category: create-microlearning-modules
position-in-category: 5
video_url: "none"
---

This page contains:

- <a href="#overview">Overview</a>
- <a href="#vsc">Install and set up Visual Studio code</a>
- <a href="#fork">Create a new fork</a>
- <a href="#clone">Clone the fork</a>
- <a href="#scaffolding">Create scaffolding with VSC extension</a>
- <a href="#branch">Create a branch</a>
- <a href="#files">Work with markdown and YAML files</a>

## Overview<a name="overview"></a>

Toward the end of development, the MLS moves all the module content into a fork in GitHub. Here's an overview of the steps. The MLS:

1. Installs and sets up Virtual Studio Code (VSC) on their computer.
1. Creates a copy (a *fork*) in GitHub of the existing [**MicrosoftDocs/learn-pr**](https://github.com/MicrosoftDocs/learn-pr) repository (*repo*).

    - The module content during development exists in this new MLS fork. 
    - The MLS doesn't ever merge this MLS fork back into the MicrosoftDocs/learn-pr fork. This is done by Microsoft after development and final sign-off.

1. Creates a copy (*clones*) the MLS fork, using VSC, to their own computer.
1. Creates the folder structure and files for all the files in the published module (called *scaffolding*) using a VSC extension.

1. Creates the unit markdown files using the text from the module doc and a program called Typora.
1. Fills in the additional information, or *metadata*, to files that were created automatically when the scaffolding was created.

    > **Tip:** The Module template has notes to guide the MLS when adding metadata to the .yml files.

The rest of this page gives high-level instructions for the MLS. It walks the MLS through the process of setting up their computer and GitHub, with the end result of having scaffolding for the module and a fork, branch, and pull request.

## Install and set up Visual Studio Code<a name="vsc"></a>

Visual Studio Code (VSC) is used to work with the module files.

- The module unit files are in a code language called *markdown*, which is similar to HTML. Markdown files have the .md extension. 
- The YAML files have the .yml extension. They are used in the published course to provide information about the course.
- Other files include images and graphics. These will have either a .png or .svg.

### What the MLS should install

As the MLS, you should install:

- [Visual Studio Code](https://waypointventures.github.io/docs/install/install-vsc.html) to edit markdown and other module files. 
- [Docs Authoring Pack](https://waypointventures.github.io/docs/install/install-author-pack.html) to expand VSC with markdown-specific tools like a spell checker, markdown syntax, and the [Docs Scaffolding extension](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-scaffolding).
- [Word Count extension](https://waypointventures.github.io/docs/install/install-wordcount-ext.html) to display a word count in open markdown files.

## Create a new fork<a name="fork"></a>

To create a fork (copy) of the MicrosoftDocs/learn-pr repo in your GitHub account: 

1. In a browser, log in to GitHub and then navigate to the MicrosoftDocs/learn-pr repo.

    > **Note:** As of this writing, to access the MicrosoftDocs/learn-pr code repo, your GitHub and v- accounts need to be linked. Refer to the instructions at [GitHub account setup](https://review.docs.microsoft.com/en-us/help/contribute/contribute-get-started-setup-github?branch=master).

1. Select the **Fork** button and then confirm your GitHub account as the location for the new fork.

    ![The Fork button in GitHub](../assets/images/github-create-fork.png)

> For more detailed information, refer to [Fork a repository](https://waypointventures.github.io/docs/download-files/fork-repo.html).

## Clone the fork<a name="clone"></a>

After you create a fork of the MicrosoftDocs/learn-pr repo, you'll be able to access and work on your fork from your computer using VSC. You do this by creating a local copy of the fork on your computer called a *clone*. You make changes to the clone (on your computer) and then periodically upload the changes to the fork in GitHub.

1. Make sure you are in your fork, the one you made from the MicrosoftLearn/learn-pr repo.
1. Select the **Code** button and then select the **Copy** button. This copies the address of your cloned repo into your clipboard. Note that when you clone, you are cloning from the root of your branch. 

    ![The Fork button in GitHub](../assets/images/github-create-clone.png)

1. Switch to VSC on your computer.
1. Select **View** > **Command Pallette** > **Git: Clone**.
1. **Ctrl+V** to paste the address of the cloned repo and then press Enter.
1. Navigate to a folder on your computer and then select **Select Repository Location**. To avoid overly-long file paths, it's suggested to create a folder directly on your C drive for the repo, for example, C:\repo-folder.

A copy of the module folder and all its contents is created on your computer. To work in VSC, open this local folder. 

### Invite collaborators

The MLS can also invite collaborators to the fork and/or branch so others on the team can also work in the fork and/or branch, if necessary. Collaborators would typically include the PjM and SME.

> For more information, refer to [Invite  a collaborator](https://waypointventures-my.sharepoint.com/personal/karinca_waypoint_ws/Documents/Invite collaborator).


## Create scaffolding with VSC extension<a name="scaffolding"></a>

To create scaffolding automatically, be sure the **Docs Authoring Pack for VS Code** extension for VSC is installed.
This extension includes the **Docs Scaffolding** extension which the MLS uses to auto-generate (*scaffold*) a skeleton module based on one of the standard module patterns:

- [Standard](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-standardmodules)
- [Introduction](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-intromodules)
- [Choose](https://review.docs.microsoft.com/en-us/help/learn/id-guidance-choosemodules)
 
> **Tip:** Before creating the scaffolding, update your Settings to auto-populate metadata when you create scaffolding for a new module. From the VSC File menu, select **Preferences**, **Settings**.
Expand **Extensions** and then select Docs Scaffolding Extension Configuration. Complete instructions can be found in VSC under **Extensions** > **docs-scaffolding** > **Details**.

![scaffolding read me](../assets/images/vsc-scaffolding-info.png)

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

For more detailed information, refer to:
-  <a href="https://waypointventures.github.io/docs/add-content/scaffold.html) or [Create scaffold template](https://review.docs.microsoft.com/en-us/help/learn/create-scaffold-template?branch=main" target="_blank">Create scaffolding ![external link](../assets/images/extlink.png)</a>.
- <a href="https://review.docs.microsoft.com/en-us/help/learn/create-scaffold-template?branch=main" target="_blank">Scaffold a module using the Docs Scaffolding extension for VS Code ![external link](../assets/images/extlink.png)</a>.


## Create a branch<a name="branch"></a>

You can make changes directly to the fork, but a method that generates a "before and after" for your changes involves a branch and pull request.

In VSC, the MLS creates a branch to use for content changes and updates. Changed content is changed in the branch, not directly in the fork. 

After making changes to files in VSC, the MLS saves and uploads the changed files to GitHub. The first time this is done, VSC will prompt the MLS to create a Pull Request.

In the pull request, you can view the changes you've made before they are merged into the fork. After the changes are reviewed in a pull request, the changed content in the branch is merged into the fork, thereby updating the fork. At this point, typically the pull request is closed and the branch is deleted.

> For more information about branches, refer to [Create a new branch in VSC](https://waypointventures.github.io/docs/branches/new-branch.html)


## Work with markdown and YAML files<a name="files"></a>

Each unit in the module must have both a markdown (.md) and a YAML (.yml) file. The files should be numbered in the order they appear in the module.

The unit markdown files contain the content of the unit. The MLS adds this content from the Module Word document by using Typora. 

The scaffolding YAML files contain placeholder text the MLS replaces with the real information from the Design or Module Word documents. Each YAML file also has one line that includes the file name for the associated markdown file.

> **Tip:** The Microlearning combined template.dotx file has comments to help the MLS move the information from the template to the YAML files.

> More detailed instructions for this process are in [Create markdown files]({{site.baseurl}}/get-started/create-markdown-files.html).

### Save and upload (push) your changes

When you save your changes in VSC, the local files are updated. 

To upload the changed local files to update the fork online in GitHub, you'll need to stage, commit, and push your changes:

1. Select the **Source Control** button.
1. Select the **Stage All Changes** (+) button to stage all changed files.
  ![stage changes buttons in VSC](../assets/images/vsc-stage-changes.png)
1. Enter a short note about the change.
1. Select the **Commit** button (the checkmark) to commit all staged changes.
  ![commit changes buttons in VSC](../assets/images/vsc-commit-changes.png)

1. Select the **Views and More Actions** button, and then select Push.
  ![push changes buttons in VSC](../assets/images/vsc-push-changes.png)

> For more detailed information about staging and pushing changes, please refer to [Send (push) files: Stage, commit and push to remote repo](https://waypointventures.github.io/docs/branches/push-files.html)
