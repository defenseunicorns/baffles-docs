# Zarf - Docs Site

[![Zarf Slack Channel](https://img.shields.io/badge/k8s%20slack-zarf-40a3dd)](https://kubernetes.slack.com/archives/C03B6BJAUJ3)
[![Zarf Website](https://img.shields.io/badge/web-zarf.dev-6d87c3)](https://zarf.dev/)
[![Zarf Documentation](https://img.shields.io/badge/docs-docs.zarf.dev-775ba1)](https://docs.zarf.dev/)

This is the docs site for [Zarf](https://github.com/defenseunicorns/zarf), a declarative air gap solution for Kubernetes.  This site is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator created by Facebook.

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

### Running

There are two ways to run the site locally, the simplest being the following:

```shell
$ npm run start
```

This will open a browser window that will let you see the built site.

> ⚠️ *Note, `npm run start` will not perform link checking or build the search index.*

To perform a full build and to run it locally you should run the following:

```shell
$ npm run build
$ npm run serve
```

### Deployment

To deploy the site, push your changes into a branch and open a PR.  [Netlify](https://www.netlify.com/) will generate a preview for you and a PR approver to see your changes.  Once the approver is happy with the changes they can approve and merge the PR and it will be pushed to production.
