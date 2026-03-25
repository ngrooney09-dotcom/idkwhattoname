# Introduction

This user guide will demonstrate the basics of working with [GitHub](https://github.com) using [Git](https://git-scm.com/docs).  
In this documentation we will go over creating a new repository in GitHub, pushing an existing project into it, and working with an existing repository (someone else's code) in GitHub.

!!! note

    :material-github: **GitHub** is a website that lets you host **git** repositories. It is used for collaboration with other developers, storing and reviewing code.

    :material-git: **Git** is a Version Control System used to track files and changes in your code over time.

## Intended Users && Prerequisite Knowledge

This documentation is intended for individuals who have a basic knowledge of GitHub such as `git clone`, `git status`, `git add`, `git commit`, `git push` etc or Version Control Systems such as Git.

## Software Requirements

The following software(s) must be installed and accounts created:

- [Visual Studio Code](https://code.visualstudio.com/download)
- [Git Bash](https://git-scm.com/install/windows)
- [GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)

## Procedures Overview

This document will cover the following tasks:

- Connecting Gitbash to Visual Studio Code terminal
- Creating a new repository in GitHub
- Pushing an existing project to  GitHub
- Working with existing code on GitHub
  - Cloning
  - Zip download

## Typographical Conventions

1. There will be no code blocks in this documentation. Screenshots will be used to guide users.
2. Filenames will be formatted in monospace code format and put in  quotes.(`package.json`)
3. Action verbs and UI elements will be bold. (**Click**, **Highlight**, **New Repository** etc)

## Notes and Warning Messages

This documentation will use message blocks to inform you of relevant information

!!! warning "Warning"
    Specifies content that must be read before proceeding.

!!! info "Info"
    Indicates additional information or tips.

!!! success "Success"
    Indicates what success looks like.