---
layout: page
title: The publishing phase
subtitle:
description: An overview of the publishing phase of a microlearning module-creation project
author: kcarlson
date: 09 Sept 2021
post-number: 3.4
category: project-info
position-in-category: 4
video_url: "none"
---

## Convert content to markdown and move to GitHub

Prior to Compliance testing, the MLS moves the module files to GitHub.

Most of the development process happens in Word, so authors and reviewers can take advantage of Word’s excellent commenting and tracking features. Just before pre-publishing tests, the MLS uses Typora to convert the module Word files to markdown. 

The MLS opens the markdown files in VSC and performs a global review and conducts remediation, including fixing bulleted lists and checking for correct syntax including headings, tables, images, and links. The MLS then uploads the markdown files to GitHub.

## Compliance testing

The MLS performs the Compliance testing pass, where they assess the content for issues in the areas of accessibility, global readiness, licensing, and privacy. The MLS corrects any issues found.

>**Note:** When in doubt, please escalate questions to the Compliance team via your PjM. 

## MLS creates a pull request from the MLS branch

After the files are uploaded to GitHub, the MLS creates a [pull request](https://waypointventures.github.io/docs/workflow/terminology.html#using-prs) to merge their branch back into the master branch. Read more about [pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

> **Important!** The MLS *should never merge* their branch into the master branch. The PjM performs this action just prior to publication.

## Quality tests

The MLS performs all content testing in this phase to ensure the module is ready for publication. 

>**Note:** To perform quality tests, the MLS must link their v-dash to their GitHub account so as to have the requisite permissions to perform these steps.

After the MLS create the pull request (refer to the previous step), anytime files are changed or added to GitHub, such as when you push changes from VSC, several automatic checks occur and are reported via email to the pull request’s owner. The automatic checks include generation of an Acrolinx scorecard with a score for each file (markdown and yaml) and a Validation (build) status, which sent to the MLS as emails.

### Acrolinx Scorecards

Acrolinx Scorecards provide detailed information about how your markdown and yaml content meets defined standards and requirements, providing metrics whereby you can improve your Acrolinx scores prior to publication. At a minimum, all Learn content must have a minimum Acrolinx score of 80. However, at Waypoint, we encourage you to strive for a score of 100 for all files.

The Acrolinx program scans all markdown and yaml files and then provides a detailed report about issues it finds, including spelling errors, sentences that are too long or complex (it likes them short and snappy—no compound sentences), word choices (it prefers simple words), and passive construction.

>**Note:** Please review all Acrolinx results, even if a file has a score above 80, to determine whether it’s flagged any spelling errors. If spelling errors are by design, such as a product name or code snippet, the PjM should make a note to that effect in the “#sign-off” comment during the publication phase. 

![Example of an Acrolinx scorecard.](../assets/images/02-projects/acrolinx-scorecard.png)

>**Hint:** To see details about the score for a particular file, select **link** in the **Scorecard** column.

### Validation (build) status

This automated check determines whether files are working correctly together to create a “finished” module. For example, in each .yml file, there’s a path for the corresponding markdown file. If the markdown file is not named correctly, this test returns an error.

- To view a detailed report for any file, click its hyperlink. 

- To preview the module as it will look in its published form, select the **View** link for the index.yml file. This will open the first page in the course. Selecting the **View** link for another page will open that page.

![Validation (build) status report.](../assets/images/02-projects/validation-status.png)

The MLS checks the automated build reports and ensures that all content can publish without errors.

The MLS checks the Acrolinx scorecard and Validation (build) status emails for problems and fixes them in the appropriate .md or .yml files.

## Publishing

Once all units of a module have an Acrolinx score of 80 or higher and pass all build-validation tests, the MLS hands off the module to the PjM, who then submits it to Microsoft for their publishing process:

1. The PjM adds “#sign-off” to the comments in the pull request.
2. The pull request gets assigned to the appropriate Microsoft reviewer.

    ![Pull request with project manager's comments.](../assets/images/02-projects/pull-request-pjm-comments.png)

3. The Microsoft Reviewer responds with feedback in comments.

    ![Pull request with Microsoft reviewer's response to project manager comments.](../assets/images/02-projects/ms-reviewer-respond-pjm-comments.png)

4. The PjM resolves the issues raised in the Microsoft reviewer’s comments.
5. The PjM comments and adds “#sign-off” in comments in the pull request.

{% include paginator.html %}