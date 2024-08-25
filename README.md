# Getting started
After installing the theme successfully it requires a just a few more steps to get your site running.

## Update config file
Copy the config.toml in the exampleSite to the root of your Hugo site. Change strings as you like.

## Check your site
In order to see your site in action, run Hugo's built-in local server.
```
npm run start
```

Now enter localhost:1313 in the address bar of your browser.

Build your site
```
npm run build
```


## Contribution Guide for the First Open-Source Job Board

### Introduction
Thank you for your interest in contributing to the first open-source job board. This guide will walk you through the steps to add new content, including how to manage tags, categories, and metadata for job postings or other content.

### Adding Content
To add new content, you'll need to create a new Markdown file in the appropriate directory. The filename should be descriptive and follow the format `YYYY-MM-DD-title.md`.

### Metadata Structure

At the top of your Markdown file, you'll include a section of metadata, also known as front matter, which is written in YAML format. Here is an example:

```yaml
---
author: "Wamo"
title: "Image Test"
image: "img/prism.jpg"
draft: false
date: 2020-08-14
description: "Image Test"
tags: ["themes"]
archives: ["2020/08"]
---
```

Let’s break down each part:

- **author**: This field should contain the name or username of the person who authored the content. This helps to give credit to contributors and allows others to know who to reach out to if they have questions or feedback.

- **title**: The title of your post. Make sure it is descriptive and relevant to the content. It will be displayed prominently on the job board.

- **image**: The path to an image associated with the post. This image could be a company logo, a related graphic, or anything that visually represents the content. Make sure the image is stored in the correct directory, usually under `img/` or a similar folder.

- **draft**: Set this to `false` if the content is ready to be published. If you're still working on it, set it to `true`. Drafts are not displayed on the live site.

- **date**: The publication date of the post. The format is `YYYY-MM-DD`. This helps to keep the job postings organized chronologically.

- **description**: A brief summary or description of the content. This will appear in previews or listings on the job board and helps users quickly understand the nature of the job or content.

- **tags**: A list of tags related to the content. Tags help users find posts related to specific topics or skills. For example, you might use tags like `["remote", "full-time", "JavaScript"]`. Make sure to use existing tags when possible to maintain consistency.

- **archives**: This is a way to organize content by date, often used to archive older posts. The format `["YYYY/MM"]` helps in categorizing posts based on the year and month they were published.

### Adding Tags and Categories

**Tags** are keywords or labels that categorize the content. To add tags, simply list them under the `tags` field in the metadata section. Separate each tag with a comma, and enclose the entire list in square brackets.

Example:
```yaml
tags: ["Php", "Android", "JavaScript"]
```

**Categories** work similarly to tags but are often broader in scope. If your job board uses categories, you can add them in a similar way:

Example:
```yaml
categories: ["Full-Time", "Freelance", "Part-Time", "Contract"]
```

If categories are not set up, you can ignore this step. Tags are usually sufficient for most job board needs.

### Finalizing Your Contribution

1. After adding your content and metadata, double-check for any errors or missing fields.
2. Ensure your image is correctly linked and located in the appropriate directory.
3. Save the Markdown file in the correct location, typically under a directory named `posts/` or something similar.
4. Commit your changes to the repository and submit a pull request (PR) with a clear description of your contribution.

### Review Process

Your submission will be reviewed by maintainers or other contributors. If any changes are needed, you'll receive feedback in the PR comments. Once approved, your content will be merged and published on the job board.

Thank you for contributing to the first open-source job board! Your efforts help connect developers and companies in meaningful ways.

