# Baffles - Docs Site

[![Baffles Website](https://img.shields.io/badge/web-baffles.dev-6d87c3)](https://baffles.dev/)
[![Baffles Documentation](https://img.shields.io/badge/docs-docs.baffles.dev-775ba1)](https://docs.baffles.dev/)

This is the docs site for [Baffles](https://github.com/defenseunicorns/baffles), a declarative air gap solution for Kubernetes.  This site is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator created by Facebook.

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

### Prerequisites

This site requires `nodejs` and `npm` so install it if you haven't already.

```shell
# FOR LINUX (Ubuntu)
$ sudo apt update
$ sudo apt install nodejs
$ sudo apt install npm

# FOR MAC (Homebrew)
$ brew install nodejs
```

### Installation

To install required dependencies run the following:

```shell
$ npm i
```

### Updating Baffles `docs` Files

The markdown files for Baffles are held in the main Baffles repo and are pulled into this repo using a submodule.  To update the reference to those docs run the following command:

```shell
$ git submodule update --remote --recursive master
```

You may also find it useful to switch to a different branch for the submodule.  You can do this by adding a `branch` to `.gitmodules`:

```
[submodule "master"]
	path = master
	url = https://github.com/defenseunicorns/baffles.git
    branch = <your-branch-here>
```

### Running

There are two ways to run the site locally, the simplest being the following:

```shell
$ npm run start
```

This will open a browser window that will let you see the built site.

> ⚠️ *Note, `npm run start` will not perform some link checking or build the search index.*

To perform a full build and to run it locally you should run the following:

```shell
$ npm run build
$ npm run serve
```

### Deployment

To deploy the site, push your changes into a branch and open a PR.  [Netlify](https://www.netlify.com/) will generate a preview for you and a PR approver to see your changes.  Once the approver is happy with the changes they can approve and merge the PR and it will be pushed to production.
