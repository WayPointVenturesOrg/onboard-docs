---
layout: page
title: Pre-publish automatic checks
subtitle:
description: Automatic checks that occur after a pull request is made - Acrolinx and Validation build status
author: kcarlson
date: 04 Nov 2021
post-number: 4.4
category: create-microlearning-modules
position-in-category: 4
video_url: "none"
---

Once a pull request exists, anytime the files in GitHub are updated, several automatic checks occur to ensure that all content can publish without errors. The automatic checks include:

- An Acrolinx scorecard with a score for each markdown and yaml file. Acrolinx checks for spelling, grammar, writing style, and terminology.
- A Validation (build) status report that tests the markdown and yaml files for various code that connects the files when the module is published. Issues found in the status report must be fixed so the module can publish correctly.

The results of these tests are reported through emails to the pull request’s owner (the MLS). The MLS checks the emails for problems and then fixes the appropriate .md or .yml files.

#### Acrolinx Scorecards

The Acrolinx program scans all markdown and yaml files and then provides a detailed report about issues it finds, including spelling errors, sentences that are too long or complex (it likes them short and snappy—no compound sentences), word choices (it prefers simple words), and active construction.

Acrolinx Scorecards provide detailed information about how the markdown and yaml content meets defined standards and requirements. The scorecards provide metrics you can use to improve the Acrolinx scores prior to publication. At a minimum, all Learn content must have a minimum Acrolinx score of 80. However, we encourage you to strive for a score of 100 for all files.

To help achieve a high Acrolinx score:

- Make sure there aren’t any misspelled words.
- Avoid compound sentences. Break apart any long sentences into smaller ones.
- Avoid overly-complex words if a more common word would do.
- Ensure there are no orphaned files in the authoring repo.

>**Note:** Review all Acrolinx results, even if a file has a score above 80, to determine whether it’s flagged any spelling errors. If spelling errors are by design, such as a product name or code snippet, the PjM should make a note to that effect in the “#sign-off” comment during the publication phase.

>**Hint:** To see details about the score for a particular file, select **link** in the **Scorecard** column.

![Example of an Acrolinx scorecard.](../assets/images/acrolinx-scorecard.png)

>**Tip:** You can install and run an Acrolinx extension in VSC to preview your Acrolinx score while you work. <a href="https://review.docs.microsoft.com/en-us/help/contribute/contribute-get-started-setup-acrolinx-vscode" target="_blank">Learn more about installing the Acrolinx extension here ![external link](../assets/images/extlink.png)</a>.

#### Validation (build) status

This automated check determines whether files are working correctly together to create a “finished” module. For example, in each .yml file, there’s a path for the corresponding markdown file. If the markdown file is not named correctly, this test returns an error.

- To view a detailed report for any file, click its hyperlink. 

- To preview the module as it will look in its published form, select the **View** link for the index.yml file. This will open the first page in the course. Selecting the **View** link for another page will open that page.

![Validation (build) status report.](../assets/images/validation-status.png)

{% include paginator.html %}
