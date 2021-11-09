---
layout: page
title: Module-writing guidance
subtitle:
description: Guidance to follow when you write a microlearning module
author: kcarlson
date: 02 Nov 2021
post-number: 4.2
category:  create-microlearning-modules
position-in-category: 2
video_url: "none"
---

This documentation is intended to give you a high-level understanding of how microlearning courses are different than ILT or other types of courses you’ve worked on in the past. It details form factors and guidance taken largely from the <a href="https://review.docs.microsoft.com/help/learn/?branch=main" target="_blank">Microsoft Learn Contributor Guide ![external link](../assets/images/extlink.png)</a>. For more specific guidance, follow the links throughout this material to specific pages from the  <a href="https://review.docs.microsoft.com/help/learn/?branch=main" target="_blank">Contributor Guide ![external link](../assets/images/extlink.png)</a>.

This page contains:

- <a href="#contentdev">Content development tools</a>
- <a href="#style">Microlearning writing style</a>
- <a href="#specific">Writing guidance for specific content</a>
- <a href="#references">References</a>

## Content development tools<a name="contentdev"></a>

Before you begin writing a module, make sure you have the [content development tools]({{site.baseurl}}/get-started/content-development-tools.html) you will need.

## Microlearning writing style<a name="style"></a>

This section details some expectations for writing which are particular to Microsoft and/or Microlearning.

### Writing is task-focused and scenario-based

Modules must be organized around job tasks. Write the module to illustrate completing a task, rather than only discussing the topic. 

Modules must include conceptual learning content; they can't solely be a walk-through.

Modules must be standalone; that is, they must be able to exist in multiple learning paths. For example, exercises should not span across modules.

Microlearning modules are scenario-based:

- You’ll write a <a href="https://review.docs.microsoft.com/help/learn/id-guidance-scenarios?branch=main" target="_blank">scenario ![external link](../assets/images/extlink.png)</a>for the introduction unit that sets the stage: the job role of the learner (for example, a database admin), the issue or problem they need to solve (for example, ensuring security while deploying a database in the cloud), and the product(s) needed to solve that problem. 

-  Make the scenario a compelling, important problem. 

-  Make it specific where possible, to add real-world dimension.

-  At the end, bring the student into the scenario with action. 

- Use the scenario in examples in the core content to illustrate how the topic manifests in the real world. Use it to illustrate the various tools, tasks, and skills the learner needs to solve their problem. 

- In the Summary unit, the initial scenario issue is restated, along with what the learner has learned in the module and how that learning solved the issue.

- When writing about a product, remember to write about the task or problem the product will solve for the learner. Use the scenario, if applicable.

### Do not plagiarize

Content cannot be copied directly from other sources such as <a href="https://docs.microsoft.com/" target="_blank">https://docs.microsoft.com ![external link](../assets/images/extlink.png)</a>.

- Although we often receive permission to re-use content, this is NEVER permission to copy and paste. Copying and pasting content is plagiarism; our customers can cancel contracts if we fail their scans for plagiarized content. 

- You can reuse content from Microsoft sources (primarily <a href="https://docs.microsoft.com/" target="_blank">Microsoft Docs ![external link](../assets/images/extlink.png)</a> and Azure Marketplace) if you always put the content in your own words and never copy and paste the content. 

- Also, you must update graphics found on these sites so the graphics meet Learn standards. 

### No marketing

Avoid marketing speak and jargon. Your writing should factual, rather than opinion or marketing. 

### Voice

Use a warm and direct voice, <a href="https://review.docs.microsoft.com/help/contribute/writing-principles-everyday-words?branch=main" target="_blank">using everyday words ![external link](../assets/images/extlink.png)</a> when possible. For example:

- Instead of this: “execute the program” 

- Write this: “run the program”

### Accessible and inclusive language

Use accessible and inclusive language. For example:

- Use “Select OK” instead of “Click OK.” 

- Don’t use words that are sensory-related like see, view, or hear, unless they are part of a UI element.

- Don’t use gendered pronouns. For example, instead of “I asked him how he would install the software.” Use, “I asked the administrator how they would install the software.”

- Don’t refer to the location of UI items with vision-oriented directions such as “left” or “right.” “After” and “before” are okay to use.

- Don’t use terms that include the word <a href="https://review.docs.microsoft.com/help/contribute/product-names-terms?branch=main" target="_blank">“master” or “slave.” ![external link](../assets/images/extlink.png)</a>

- Content can't violate any <a href="https://review.docs.microsoft.com/help/contribute/contribute-legal-guidelines" target="_blank">legal ![external link](../assets/images/extlink.png)</a> or <a href="https://review.docs.microsoft.com/help/contribute/contribute-accessibility-guidelines" target="_blank">accessibility standards ![external link](../assets/images/extlink.png)</a>.

### Less is more

Write about the primary idea and get to the point quickly. Microlearning shouldn’t and can’t cover everything that the ILT course would cover. Check out <a href="https://styleguides.azurewebsites.net/Styleguide/Read?id=2700&topicid=28939" target="_blank">Microsoft Writing Style Guide, Top 10 tips for Microsoft style and voice ![external link](../assets/images/extlink.png)</a>. For example:

- Instead of this: “The Recommended Charts command on the Insert tab recommends charts that are likely to represent your data well. Use the command when you want to visually present data, and you're not sure how to do it.”

- Write this: “Create a chart that's right for your data by using the Recommend Charts command on the Insert tab.”

### Break up text 

Break up text by adding headings, notes, lists, tables, screenshots, and diagrams. A well-crafted unit contains 1-2 diagrams and/or screenshots as well as notes. You can use up to four diagrams and/or illustrations per unit.

>**Note:** Limit your use of screenshots. They can prematurely “age” courses as products advance and the UI changes. 

Provide the MP (Media Production) in the team with a sketch or similar drawing as soon as you know you need it so they can create an appropriate graphic. 

Ensure you add alt-text to every graphic and screenshot. 

Complex images should be explained in the body of the text, not in the alt-text. In addition, graphics must supplement the text; they shouldn’t be the *only* way that content in conveyed. The text must explain the concepts that the graphics illustrate.

>**Important:** Remove or replace any personally-identifying information from screenshots. In the past, it was allowable to blur this information, but the current requirement is that the information be removed or replaced with fictitious names and information.

## Writing guidance for specific content<a name="specific"></a>

### Alerts

Use alerts to convey tidbits of tangential information or warnings. You can use note, tip, important, caution, and warning. 

> For more information, refer to <a href="https://review.docs.microsoft.com/help/contribute/markdown-reference?branch=main" target="_blank">Docs Markdown reference ![external link](../assets/images/extlink.png)</a>.

![preview of alerts](../assets/images/preview-alerts.png)

### Videos

Modules may include a short conceptual video by customer request. They are sometimes offered in lieu-of graphics or exercises when those tools will not suffice to educate learners. 

In Microlearning courses, videos are concept-based and are developed by and provided by Microsoft. You can replace an exercise with a skill demonstration video. 

>**Important:** Keep in mind that in the past, these videos have taken 6-8 weeks to deliver. 

To obtain a demonstration video, provide a 300-words-or-less “directorial guidance” document to Microsoft. They create desktop demonstration videos that have captions. Microsoft then publishes the video to Red Tiger.

>**Note:** 

Red Tiger will be replaced with a different platform by the end of quarter 2, 2021.

> For more information, refer to  <a href="https://review.docs.microsoft.com/help/contribute/contribute-video-create?toc=/help/learn/toc.json&bc=/help/learn/breadcrumb/toc.json&branch=master" target="_blank">Create and Publish Video ![external link](../assets/images/extlink.png)</a>.

### Code samples

Code samples should include multiple programming languages. If you have coding exercises, they should ask the learner to write some original code (that is, not solely cut-and-paste).

![code sample](../assets/images/code-sample.png)

### Publishing

Content must meet the <a href="https://review.docs.microsoft.com/help/contribute/contribute-how-to-write-pull-request-quality-criteria?toc=/help/learn/toc.json&bc=/help/learn/breadcrumb/toc.json&branch=main" target="_blank">PR (Pull request) quality criteria ![external link](../assets/images/extlink.png)</a> in the <a href="https://review.docs.microsoft.com/help/learn/?branch=main" target="_blank">Microsoft Learn Contributor Guide ![external link](../assets/images/extlink.png)</a>. 

Each published file must have a minimum Acrolinx score of 80. To help achieve a high Acrolinx score:

- Make sure there aren’t any misspelled words.

- Avoid compound sentences. Break apart any long sentences into smaller ones.

- Avoid overly-complex words if a more common word would do. 

- Ensure there are no orphaned files in the authoring repo.

### Links

Links must be to an approved source, which is typically Microsoft or Azure. 

Only include links in the **Summary** unit. Don’t include them in any other unit unless they are needed to set up an environment for an exercise. 

### Definitions of terminology

Include definitions for all introduced terminology. Include definitions for all acronyms the first time they’re used.

### Fictitious names

Individual and company fictitious names used in examples or exercise must be taken from the <a href="https://microsoft.sharepoint.com/sites/lcaweb/Pages/Applications/FictitiousNameFinder.aspx" target="_blank">Microsoft CELAWeb Approved fictitious names & guidelines ![external link](../assets/images/extlink.png)</a>. Your Project Manager will acquire and provide a list for you to use at the beginning of the project.

### Third-party references 

In general, avoid references to third-party products, websites, logos, etc., in both text and graphics. Contact your PjM for specific information about the module you’re working on.

> For more information, refer to <a href="https://review.docs.microsoft.com/help/contribute/contribute-legal-guidelines?branch=main" target="_blank">Legal guidelines ![external link](../assets/images/extlink.png)</a>.

#### Third-party references that are not okay to use

Don’t use one specific third-party product to represent a category of products. For example, don’t write: “Easily cross-post to services such as Instagram.” Removing the third-party product name makes this sentence okay: “Easily cross-post to social media.”

Don’t list only some product names and not others because you don’t have room to list all the products in the category. This can give the appearance of endorsing the products you list. Instead, link to an approved Microsoft site that includes the list. Alternatively, you can provide instructions for finding the complete list in the UI of the Microsoft product (if applicable).

#### Third-party references that are mostly okay to use

Providing that the third-party product or company name used does not seem to endorse the product or company over other products or companies, it’s okay to use third-party references when:

- The reference is to an open-source products or tools that are frequently considered critical to using the Microsoft product.

- The reference is to a third-party product that “actively contributes” to the understanding of the Microsoft product.

#### Third-party references that are okay to use

It’s okay to use third-party references when:

- The content is explicitly teaching how to use a third-party product.

- The third-party product is “built-in” to an Azure product or service.

- A hyperlink to an approved Microsoft website uses the product name in the link and/or the webpage title.

## References<a name="#references"></a>

- Condensed version of all the detailed guidelines for Learn modules: <a href="https://review.docs.microsoft.com/help/learn/id-guidance-checklist?branch=main" target="_blank">Detailed guidelines quick reference ![external link](../assets/images/extlink.png)</a>

- <a href="https://review.docs.microsoft.com/help/learn/content-requirements?branch=main" target="_blank">Microsoft Learn deliverable requirements ![external link](../assets/images/extlink.png)</a>

- <a href="https://review.docs.microsoft.com/help/contribute/style-guide-hierarchy?toc=/help/learn/toc.json&bc=/help/learn/breadcrumb/toc.json&branch=main" target="_blank">Hierarchy of style guides - Docs Contributor Guide ![external link](../assets/images/extlink.png)</a>

{% include paginator.html %}