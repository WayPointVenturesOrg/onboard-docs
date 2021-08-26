---
layout: page
title: Example guide
subtitle:
description: An example of a guide
author: mkavana
date: 26 Aug 2021
post-number: 1.1
category: this-category
position-in-category: 1
video_url: "none"
---

An example of a guide.

## Heading example

An example of a heading and image.

![Alt text](../assets/images/01-this-category\01-example-guide/01-image.png)

## Front matter

Variable name|Options and description
:---|:---
*layout*|Options are **page** or **default**. Always set this to **page**, unless you require a full width webpage with no sidebar (like the landing/ welcome page).
*title*|Add a title. This will appear on the webpage and in the sidebar.
*subtitle*|Add a subtitle. This will appear on the webpage but not in the sidebar.
*description*|Add a description. This won't appear anywhere but is helpful to understanding what the page is about.
*author*|Add your name
*date*|Add a date for when you created the markdown file in the format `DD` `mmm` `YYYY` e.g. **01 Apr 2021**.
*post-number*|Give the post a number like **1.2** where **1.** refers to the category number (i.e. category number 1) and .2 refers to the post number within the category. So, 1.2 is the first category, second post.
*category*|Assign the post to a category. The category you assign must exist in the YAML file `_config.yml`. You can add categories to `_config.yml`, in the **Sections** list/ array.
*position-in-category*|Assign a number. This number determines where the post will appear in the sidebar, within the corresponding sidebar category.
*video_url*|Options are **none** or a url. To add a video to a page, change **video_url** from **none** to a url like **https://web.microsoftstream.com/embed/video/123**. Then add the **video include link** wherever you want the video to appear inside your markdown file. Refer to [Some guide]({{site.baseurl}}/that-category/some-guide.html).

It's also worth noting the syntax for linking to pages within this site (refer to the last cell in the previous table). Note the prefix `{{site.baseurl}}`. The prefix ensures your links will work locally and on GitHub.
