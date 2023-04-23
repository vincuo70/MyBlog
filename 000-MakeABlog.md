---
title: "How make a DevBlog"
date: 2023/04/07
---

## Some prerequisites

### Take a look to Hexo

- [Hexo](https://hexo.io/)

### Take a course on Markdown

It's a very simple markup language; it's fine to write a tech blog width it.

- [Markdown Cheat Sheet – How to Write Articles in Markdown Language](https://www.freecodecamp.org/news/markdown-cheatsheet/)
- [Markdown cheatsheet](https://github.com/zairahira/Markdown-cheatsheet/blob/main/README.md)

### Use winget

Do you know that Windows has it's own packet manager?

- [Use the winget tool to install and manage applications](https://learn.microsoft.com/en-us/windows/package-manager/winget/)

### Install Visual Studio Code and some extensions

    winget install Microsoft.VisualStudioCode
    winget install Git.Git
    winget install GitExtensionsTeam.GitExtensions
    winget install --id GitHub.cli
    code --install-extension DavidAnson.vscode-markdownlint
    code --install-extension hnw.vscode-auto-open-markdown-preview

### Install Node

    winget install OpenJS.NodeJS.LTS

### Install Hexo

    npm install hexo-cli -g

## Now let's fire

### Create workspace

Choose a parent folder, and a new child folder name for your box then

    hexo init vincuo70.github.io
    cd vincuo70.github.io
    npm install
    git clone https://github.com/theme-next/hexo-theme-next themes/next

Edit `_config.yml` as per your needs, set the theme name

### Put your content

In the source\_posts folder create a markdown file for each post of your blog. Carefully assign the file name. If the article has images, add a folder with the same name as the file and put the images inside.

### Generate and check the blog

    hexo clean
    hexo generate
    hexo server

### Publish

Note: See another theme: [Fluid](https://fluid-dev.github.io/hexo-fluid-docs/en/)

Note II: See another wheel: [kiko.io](https://kiko.io/series/a-new-blog/)
