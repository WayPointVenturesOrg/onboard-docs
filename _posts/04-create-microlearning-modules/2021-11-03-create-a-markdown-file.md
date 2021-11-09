---
layout: page
title: Create a markdown file
subtitle:
description: Notes on working in the markdown language
author: kcarlson
date: 03 Sept 2021
post-number: 4.3
category: create-microlearning-modules
position-in-category: 3
video_url: "none"
---

Markdown is a markup language that you can use to create web content in a simple word-processing format and then easily convert it to web content in HTML. It’s similar to HTML but much easier for most people to use, and we do, in many of our courses in the GitHub and Azure DevOps environments. Toward the end of our development phase, when compliance testing needs to occur (and before a module can publish), the Microlearning Specialist (MLS) converts a module Microsoft Word document into separate markdown files (one for each unit) and moves them into the GitHub environment.

Here are some specific markdown guidelines and examples. This is not a tutorial or exhaustive guide. For more specific guidance and examples, refer to the [Waypoint Markdown syntax guide](https://waypointventures.github.io/docs/add-content/syntax.html) and related pages.

## File names

Here’s an example of a correct file name: `3-use-azure-resource-manager.md`

Markdown, YML, and image file names should:

- Start with the unit number.
- Use all lowercase letters.
- Use dashes to separate the words in the name (don’t use underscore characters).
- Not use abbreviations or unapproved acronyms in file names. For Azure technologies, don’t use “rm” or “arm” in file names.
- Be less than 80 characters. If the name is longer than 80 characters, the publishing process will fail.
- Not use small words like “to” and “a” that aren’t critical to the name’s meaning.
- Approximate the unit titles, but they don’t need to be a precise match.
- Use active verbs and not use gerunds (“ing” verbs).

## Alerts in markdown

Break up your text with notes, tips, images, diagrams, tables, and lists. Alerts in markdown always start on a new line and begin with an angled backet (>). The word (note, tip, important, caution, warning) is prefaced by an exclamation point (!) and enclosed in square brackets. Do not add asterisks to add bold text. If the note is part of a list, indent the entire note.

The text you enter:

\> [!NOTE] 

\> Information the user should notice even if skimming.

\> [!TIP] 

\> Optional information to help a user be more successful.

\> [!IMPORTANT] 

\> Essential information required for user success.

\> [!CAUTION] 

\> Negative potential consequences of an action.

\> [!WARNING] 

\> Dangerous certain consequences of an action.

What the alerts look like in markdown:
:::image type="content" source="../../assets/images/notes-in-markdown.png" alt-text="Screenshot of alerts in markdown.":::

What the alerts look like in the Learn module:

:::image type="content" source="../../assets/images/preview-alerts.png" alt-text="Screenshot of alerts in markdown.":::

Please refer to [Add alerts](https://review.docs.microsoft.com/en-us/help/learn/unit-add-alerts?branch=main).

## Graphics in markdown

To insert a graphic in markdown, use:

\:::image type="content" source="../../media/image.png" alt-text="Alt text here." border="false":::

To insert a screenshot in markdown, use:

\:::image type="content" source="../media/image.png" alt-text="Alt text here.":::

>**Note**: Screenshots require a border. The border property defaults to true (meaning there is a border by default), so you don't need to specify it explicitly.

>**Warning:** If you copy and paste from Word or other sources, you run the risk of including “curly” quotes, known as typographer quotes. Typing quote marks directly in a markdown file in Visual Studio Code (VSC) or GitHub will insert the correct straight quotes. 

Other important points about graphics include:

- If you’re adding a graphic in, or after, a list or other indented text, indent the paragraphs in markdown and the graphic will align with the list. 
- Screenshots should be PNG format. 
- Conceptual graphics (drawings) should be SVG format.

- Graphics should be between 800 pixels and 1200 pixels in width.
- Image file names should follow this conventional file-name structure that includes the unit number and a short description of the image. For example: **3-scale-in-out.png**.
- All images must have alternative text or be marked as decorative, meaning they don’t convey information necessary to learning. Icons don’t require alt text but must be marked as decorative. To mark items as decorative, use the :::image::: [markdown extension](https://review.docs.microsoft.com/en-us/help/contribute/markdown-reference#images) with type="icon", which will output an empty alt attribute. 
- Put images in the media folder.

:::image type="content" source="../../assets/images/media-folder.png" alt-text="Screenshot the media folder.":::

Refer to [Create and format screenshots in documentation](https://review.docs.microsoft.com/en-us/help/contribute/contribute-how-to-create-screenshot?toc=/help/learn/toc.json&bc=/help/learn/breadcrumb/toc.json&branch=main).

>**Note:** You can see graphics in a Preview tab in VSC only if you have the [Docs Authoring Pack](https://review.docs.microsoft.com/en-us/learn-docs/docs/install-authoring-tools) installed. Graphics and alerts won’t be visible in GitHub; you’ll see the code instead of a preview. The following screenshot depicts how graphics and alerts appear in GitHub.

:::image type="content" source="../../assets/images/github-how-graphics-and-alerts-appear.png" alt-text="Screenshot of what preview looks like in GitHub.":::

## Alt text

Make sure that all graphic files are in the media folder and are named appropriately. Replace the “All text here.” text with appropriate alt text. If the graphic is conceptual and the concepts it communicates are adequately described in the surrounding text (which is ideal), the alt text only needs to identify the graphic. Remember that sighted users usually don’t access the alt text and likely won’t be helped by your description of the graphic.

## Lightbox

We recommend that you [create a lightbox](https://review.docs.microsoft.com/en-us/help/contribute/contribute-how-to-use-lightboxes) for screenshots or conceptual graphics with small text or details. Selecting a lightboxed graphic opens the graphic in a pop-up window. This makes it easier to view small text or detail that’s hard to read otherwise. If you’re using more simple, conceptual graphics, you might not need a lightbox. The markdown syntax to create a lightbox is: 

\:::image type="content" source="../../assets/images/image-file-inline.png" alt-text="Image alt text" lightbox="image-file-expanded.png":::

>**Note:** In this example, there are two different images. One is smaller and used for the source property, while the other is larger and used for the lightbox. If the image used is larger, you can use it for both the source and lightbox. 

## Links in markdown

Reminders:

- Links must resolve to an approved source, which typically means to Azure or Microsoft content. 
- Don’t use AKA or forwarding links. 
- Only include links in the Summary unit. Typically, links aren’t included in other units unless they’re critical to setting up or configuring an environment for an exercise. 

In markdown: 

- Don’t use abbreviations in links. This can affect Acrolinx scores that result from automated build testing. 

    >**Note**: A file must achieve a minimum of an 80 Acrolinx score to publish, per the Learn platform. Waypoint’s mandate is that we’d like all files to achieve Acrolinx scores of as close to 100 as possible.

- To open a link in a new tab, add **?azure-portal=true** at the end of the URL. Note that this is case-sensitive. For example: https://docs.microsoft.com/learn/paths/explore-microsoft-azure-cloud-concepts?azure-portal=true 
- If the link contains localization, remove the **en-us**. For example, change: 
- https://review.docs.microsoft.com/en-us/help/learn/ to 

- https://review.docs.microsoft.com/help/learn/ 

## Inline code and code blocks

If you use example of computer code interspersed with other text (inline code) in your markdown file, surround the code with single tick marks (use the same key as the tilde ~). For example, in this sentence, \`this is the code`.

If you use example of computer code (code blocks) in your markdown file, use syntax highlighting to ensure it displays correctly. Do this by beginning and ending the code block with three tick marks (use the same key as the tilde ~). Also specify the computer language in which the code is written after the first three tick marks.

For example, the \```ruby and \``` that begin and end this code will display the following block of **Ruby** language programming code:  

:::image type="content" source="../../assets/images/code-sample.png" alt-text="Screenshot of Ruby code in markdown.":::

Refer to [WayPoint Ventures:Markdown syntax guide](https://waypointventures.github.io/docs/add-content/syntax.html#markdown-code-blocks) for more information. 

## Additional resources for including code

[Technical principles checklist - Docs Contributor Guide | Microsoft Docs](https://review.docs.microsoft.com/en-us/help/contribute/technical-principles-checklist?branch=main) 

Code conventions:

- [Azure CLI](https://review.docs.microsoft.com/en-us/help/contribute/conventions-azure-cli) 

- [Azure PowerShell](https://review.docs.microsoft.com/en-us/help/contribute/conventions-azure-ps) 
- [C# Coding Conventions (C# Programming Guide)](https://review.docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)
