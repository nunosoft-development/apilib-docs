# Contributing Guidelines

Welcome to the contributing guidelines for our API-Lib documentation project! We appreciate your interest in contributing and helping us improve the documentation for API-Lib.

## How to Contribute

To contribute to the documentation, follow these steps:

1. Fork the repository.
2. Clone your forked repository to your local machine.
3. Create a new branch for your changes.
4. Make your changes to the documentation files. The documentation is written using Markdown files.
5. Update the `layout.json` file to include any new pages you create.
6. Once you're satisfied with your changes, commit and push your changes to your forked repository.
7. Open a pull request to merge your changes into the main repository. 

## Writing Guidelines

When writing or editing documentation, please keep the following guidelines in mind:

- Write clear and concise explanations that are easy to understand.
- Use correct spelling and grammar.
- Use proper formatting and syntax for Markdown files.
- Ensure that your documentation is accurate and up-to-date.
- Use appropriate headings, lists, and other formatting to make the documentation easy to navigate.

## Page Routing

The file path and name of each Markdown file in the `repository` determines its page route in the documentation site. The file path and name should be in lowercase and separated by hyphens, and the file extension should be `.md`. For example, a Markdown file located at `Introduction/apilib-features.md` would have the page route `/introduction/apilib-features`.

## Navigation Layout

The `layout.json` file located in the root folder of the repository contains the navigation layout for the documentation site. When creating a new page, be sure to add it to the appropriate section in the `layout.json` file so that it appears in the navigation menu.

## Setting Page Title and Description

Each Markdown file should start with the following text to set the page title and description:

```
---
title: My Page Title
description: This is a description of my page.
---
```

Please make sure to replace `My Page Title` and `This is a description of my page` with the appropriate title and description for your page.

## Custom Tags

Custom tags are special tags that are defined by the developer to render custom components in the documentation. In this project, there are several custom tags that can be used to render different components. Here is a brief explanation of each custom tag:

1. `callout`: This tag is used to render callout components with a title and message. It has two attributes, `title` and `type`, which respectively specify the title of the callout and the type of the callout (note or warning).

Example:
```
{% callout title="Note" type="note" %}
This is a note.
{% endcallout %}
```

2. `figure`: This tag is used to render images with captions. It has three attributes, `src`, `alt`, and `caption`, which respectively specify the source of the image, the alternative text for the image, and the caption for the image.

Example:
```
{% figure src="https://example.com/image.png" alt="Image" caption="This is an image" /%}
```

3. `quick-links`: This tag is used to render a list of quick links. It has no attributes.

Example:
```
{% quick-links %}
{% quick-link title="Home" href="/" icon="HomeIcon" description="Go to the home page" /%}
{% quick-link title="About" href="/about" icon="InformationCircleIcon" description="Learn more about us" /%}
{% /quick-links %}
```

4. `grid-list`: This tag is used to render a grid of items. It has no attributes.

Example:
```
{% grid-list %}
{% grid-list-item index=0 title="Hello World" icon="GlobeAltIcon" href="/" description="The Hello World API-Lib example is a simple API that responds with the message 'Hello, World!'' when a GET request is made to its endpoint." iconForeground="text-indigo-700" iconBackground="bg-indigo-50" /%}
{% grid-list-item index=1 title="Return JSON" icon="CodeBracketIcon" href="/" description="The Return JSON API-Lib example demonstrates how to create a simple API endpoint that returns a JSON response." iconForeground="text-sky-700" iconBackground="bg-sky-50" /%}
{% /grid-list %}
```

5. `badge`: This tag is used to render a badge with a text and color. It has two attributes, `text` and `type`, which respectively specify the text for the badge and the color of the badge (red, yellow, green, blue, indigo, purple, pink, or gray).

Example:
```
{% badge text="New" type="yellow" /%}
```

## Code of Conduct

We expect all contributors to abide by our code of conduct. Please read the [Code of Conduct](https://github.com/nunosoft-development/apilib-docs/blob/production/CODE_OF_CONDUCT.md) before contributing.

## Conclusion

We appreciate your contributions to our API-Lib documentation. If you have any questions or need assistance, please reach out to the project maintainers. Thank you for helping us improve our documentation!