---
layout: page
title: The development phase
subtitle:
description: An overview of the development phase of a microlearning module-creation project
author: kcarlson
date: 09 Sept 2021
post-number: 3.3
category: project-info
position-in-category: 3
video_url: "none"
---
This page contains:

- <a href="#creation">SME creates module content</a>
- <a href="#reviews">Module reviews</a>
- <a href="#github">Work in GitHub</a>
- <a href="#autochecks">Automatic checks</a>

## SME creates module content<a name="creation"></a>

In this phase, the SME Writer (SME) writes the module content, requests conceptual graphics from our Media Production team (MPs), and develops exercise steps and/or creates a video concept document. 

>**Note:** A *video concept document* is a 300-words-or-less “directorial guidance” document provided to Microsoft to obtain a desktop demonstration video with captions. 

Here are some important items to note:

- The MLS or PjM will provide a copy of the template to the SME that is prepared for module development. 

- The SME must use the provided Module template in Word to create the module. The Module template contains the required structure and format for the module, and includes helpful notes and links to pertinent portions of the <a href="https://review.docs.microsoft.com/help/learn/?branch=main" target="_blank">Microsoft Learn Contributor Guide ![external link](../assets/images/extlink.png)</a>. Like a module’s design document, the actual module units *must conform* to the Microsoft Learn guidelines. SMEs must use the provided templates and not their own formats. 

    >**Note:** It’s imperative to use the headings and other Word paragraph styles that provided templates use. These are necessary to confirm to Learn requirements and standards, and also enable us to correctly and seamlessly convert Word files to markdown. 

- A project’s customer signs off on the completed design document. Therefore, the SME must adhere to that document. Otherwise, a Change Order is required. A PjM must administer all change orders.

- During development, the SME needs to identify the need for any conceptual graphics or demonstration videos, and work with the assigned Multimedia Provider (MP) to create these deliverables.

    >**Note:** We recommend that use of screenshots be limited. They can quickly become out of date.

- For the student “hands on” exercises, the SME determines the exercise steps and chooses one of two environments:

    1. A Microsoft Azure sandbox.
    1. A Bring-Your-Own-Subscription (BYOS), where students use their own Azure account.

- The SME should write with active voice using <a href="https://review.docs.microsoft.com/help/contribute/writing-principles?branch=main" target="_blank">Microsoft writing principles</a> and <a href="https://styleguides.azurewebsites.net/StyleGuide/Read?id=2700">Style Guide ![external link](../assets/images/extlink.png)</a>.

- For exercises or descriptions of steps, the SME should use <a href="https://styleguides.azurewebsites.net/Styleguide/Read?id=2700&topicid=29016" target="_blank">Microsoft style for procedures ![external link](../assets/images/extlink.png)</a>. They should be vigilant about using the correct full naming convention (on first reference), spelling, and capitalization of all tools, products, components, terms, and UI elements.

## Module reviews<a name="reviews"></a>

After the SME completes writing the module, the module is reviewed by several people. All of the reviews are either performed by, or reviewed by, the Microlearning Specialist (MLS). The SME must be available to the MLS to review changes and provide any needed clarifications.

The first few reviews happen using the Word module document. Then the MLS converts the module to markdown files for several pre-publishing checks.

>**Note:** For more information about the review steps that the MLS performs, refer to [MLS responsibilities]({{site.baseurl}}/people/mls.html).

>**Note:** If a module has exercises, the exercise units are sent for Functional Testing. This happens any time after completion of the exercise units and the SME effects all fixes and remediation.

### Instructional design (ID) pass

The MLS reviews the module using instructional-design principles to guide their evaluation. The MLS checks the module against the module design to ensure that all planned content is present. They also review the module for clarity of writing, terminology, correct use of Microsoft style, correct and concise exercise steps, and other items. The SME needs to be available to the MLS during the ID pass for questions and clarifications, such as terminology spelling and capitalization or procedural steps.

At this point in the process, the module is in Word, so the MLS uses track changes and comments to conduct their edits. The SME reviews the MLS edits and returns the Word document to the MLS.

>**Note:** In the past, there was a separate Instructional Designer (ID) job role. The ID pass is now performed by the MLS. 

### Copy Edit pass

After the ID pass is complete, the MLS hands off the module to the Copy Editor (CE). The CE performs a line edit of the content, reviewing for grammar, clarity, flow, and writing style and sentence structure, and also determines whether terminology and capitalization are correct for all products, terms, components, tool, and similar. The CE also helps tighten sentence structure, as complex sentences can result in low Acrolinx scores (successful publication is contingent on sufficient Acrolinx scores). CE also runs the FindWords macro and Editor tool on all content to ensure it’s compliant and correct.

Like the ID pass, the module is in Word, so the CE uses track changes and comments to conduct their edits. Once the CE finishes their pass, they submit their edited content to the MLS. The MLS resolves or rejects the tracking, and may ask the SME questions to clarify the content.

### Compliance testing

The MLS performs the Compliance testing pass, where they assess the content for issues in the areas of accessibility, global readiness, licensing, and privacy. The MLS corrects any issues found.

## Work in GitHub<a name="github"></a>

There are two more pre-publishing tests that both require that the module be converted to markdown files and uploaded to GitHub. First, the MLS prepares the location for the module and its supporting files by creating an MLS branch and adding scaffolding. They then use the Word version of the module to create markdown files which they move to GitHub. At this point, the Word module doc is no longer used and the markdown files become the working copy of the module.

### Create a new branch

In GitHub, the MLS creates an MLS branch off the master to use for the module. One branch is made per module. The MLS can create this branch through a browser in GitHub or <a href="https://waypointventures.github.io/docs/branches/new-branch.html" target="_blank">in Visual Studio Code (VSC) ![external link](../assets/images/extlink.png)</a>.

>**Note:** To access the GitHub environment, the MLS must link their v-dash to their GitHub account so as to have the requisite permissions.

The MLS creates folders and supporting .yml files, called *scaffolding*, in the MLS branch. The MLS then invites to the branch as collaborators people with the following roles:

- SME
- PjM
- CE

>**Note:** For more detailed information about any MLS task, refer to [tasks and responsibilities of the MLS]({{site.baseurl}}/people/mls.html).

>**Note:** For detailed information about using VSC and GitHub, please refer to <a href="https://waypointventures.github.io/docs/add-content/syntax.html" target="_blank">Waypoint Ventures documentation ![external link](../assets/images/extlink.png)</a>. Keep in mind that these instructions may suggest procedures that don’t align with microlearning. Contact your PjM if you have questions.

### Convert content to markdown and move to GitHub

Most of the development process happens in Word, so authors and reviewers can take advantage of Word’s excellent commenting and tracking features. Just before pre-publishing tests, the MLS uses Typora and the module (a Word file) to create markdown files. The MLS then globally checks and fixes items such as bulleted lists, headings, tables, images, and links, and uploads the markdown files to GitHub. 

> For more information, refer to [Create a markdown file]({{site.baseurl}}/create-microlearning-modules/create-a-markdown-file.html).

### MLS creates a pull request from the MLS branch

After the MLS uploads the markdown files to GitHub, the MLS creates a <a href="https://waypointventures.github.io/docs/workflow/terminology.html#using-prs" target="_blank">pull request ![external link](../assets/images/extlink.png)</a> to merge their branch back into the master branch. 

> For more information, refer to <a href="https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests" target="_blank">About pull requests ![external link](../assets/images/extlink.png)</a>.

> **Important!** The MLS *should never merge* their branch into the master branch. The PjM performs this action just prior to publication.

### Automatic checks<a name="autochecks"></a>

Once a pull request exists, anytime the files in GitHub are updated, several automatic checks occur to ensure that all content can publish without errors. The automatic checks include:

- An Acrolinx scorecard with a score for each markdown and yaml file
- A Validation (build) status report 

The results of these tests are reported through emails to the pull request’s owner (the MLS). The MLS checks the emails for problems and then fixes the appropriate .md or .yml files.

> For more information, refer to [automatic checks]({{site.baseurl}}/create-microlearning-modules/automatic-checks.html).

{% include paginator.html %}
