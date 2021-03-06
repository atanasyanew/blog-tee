# Theoretical electrical engineering blog

This repository is a home of Theoretical electrical engineering related topics

## Overview

The application is build on top of the [Hugo](https://gohugo.io/). Hugo is one of the most popular open-source static site generators (SSG), with its amazing speed and flexibility.

Improved performance, security and ease of use are just a few of the reasons static site generators are so appealing. The purpose of website generators is to render content into HTML files. Most are “dynamic site generators.”, which means it is possible to review the files locally before copying them to the computer hosting the HTTP server.

A large pool of different open source themes are written for hugo. The application uses a modified version of theme called [aether](https://themes.gohugo.io/aether/).

The content of the topics is written by ``markdown`` markup language. There are many third party solutions with user interface for content creating, such as forestry.io, instead of writing ``markdown``

The application uses a [GitHub](https://github.com/) repository for the source code files and [GitHub Pages](https://pages.github.com/) for deployment. A custom shell script is used for deployment, but this process can be optimized further more with continuous integration and continuous delivery (CI CD).

## Installing and running

Assuming git is already installed.
Hugo is easy to install, just follow the guide from the [official documentation](https://gohugo.io/getting-started/installing/).

**Hugo version used:** [v0.56.3](https://github.com/gohugoio/hugo/releases/tag/v0.56.3)

After all of the installation processes finish, the application can be run with the following command, executed inside of the terminal.

```sh
hugo serve
```

This command serve the application which is now accessible at ``localhost:1313``

## Content creation

Lightweight markup language - markdown is used for the content creation.

Typography examples are shown in the another topic.

A new post can be create by either create new file in the ``./content/post`` folder or by terminal.

```shell
hugo new post/YYYY-MM-DD-name.md
```

This command will create a new post with the default template.

## Deployment

For hosting the entire project is used the free [GitHub](https://github.com/) feature [GitHub Pages](https://pages.github.com/). GitHub Pages are hosted directly from your GitHub repository, so it is possible to just edit, push, and changes are live.

In order to deploy a shell scripts is used, basically the script build the application (generates the static content) and then commit and push the changes to the hosted git-pages branch. More information about the deploy script can be found at [Hugo documentation](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

Deployment with the script can be done with the following command executed inside git bash

```sh
 ./deploy.sh
```

Deployment process can be optimized more with the Continuous deployment technique.

There are serval Continuous deployment providers that the project can be integrate with, such as AzureDevOps and Forestry.io

## Typical use case

The following example serves locally the application in order to review our changes, creating a new topic, then commit the changes to the master branch and deploy the newly version of the generated static content.

```sh
# Navigate to the source code folder and run the project
hugo serve

# Create a new topic
hugo new post/YYYY-MM-DD-name.md

# Save and commit and push the changes
git add .
git commit -m "Added topic YYYY-MM-DD-name"
git push origin master

# Deploy
./deploy.sh
```
