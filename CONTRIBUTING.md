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

## Code of Conduct

We expect all contributors to abide by our code of conduct. Please read the [Code of Conduct](https://github.com/nunosoft-development/apilib-docs/blob/production/CODE_OF_CONDUCT.md) before contributing.

## Conclusion

We appreciate your contributions to our API-Lib documentation. If you have any questions or need assistance, please reach out to the project maintainers. Thank you for helping us improve our documentation!