
# API-Lib Docs

**[View the docs →](https://docs.api-lib.com/)**

[Contribute to the docs](https://github.com/nunosoft-development/apilib-docs/blob/production/CONTRIBUTING.md)

## Setup

Install the Node.js dependencies for this project using npm or another package manager:

```sh
$ npm install
```

## Development

When making changes to the site, including any content changes, you may run a local development server by running the following command:

```sh
$ npm run dev
```

This spawns a server that will be accessible via `http://localhost:4009` in your browser. Additionally, any changes made within the project will automatically reload your browser tab(s), allowing you to instantly preview your changes!

To see the style error(s), you may run:

```sh
$ npm run lint
```

Finally, some of these code-style errors may be fixed automatically. To do so, you may run:

```sh
$ npm run format
```

## Deployment

Our docs are deployed using API-Lib Frontend [Closed Beta]. Every commit pushed to production will automatically deploy to [docs.api-lib.com](https://docs.api-lib.com).
