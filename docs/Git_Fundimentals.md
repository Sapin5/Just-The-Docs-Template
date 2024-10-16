---
layout: default
title:  Git Fundimentals
nav_order: 3
---

<!-- prettier-ignore-start -->
# Git Fundamentals
{: .no_toc }

This page contains the basic set up and steps for configuring GIT on your local machine, as well as creating your first file

## Configure Git
In order to configure Git properly, first you must open gitbash or a terminal. After opening either, try running git --version to ensure git is installed.
Git should probably know who you are, add your email and name by running the following commands
```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
## Initializing Your First Repo
To initialize your first repo, navigate to the folder in which you would like to the main folder for your project. Create a .ignore file to ignore any files that you would not like to be tracked. Once this is done, you can run the following command:
```
git init .
```

## Staging and Commiting Files
In order to commit your files and start tracking them, you first have to stage them. This can be done by running the following command:
```
git add . 
```
Once this is run your files have been staged, but are not yet comitted. In order to commit them you can run:
```
git commit .
git commit . -m "Insightful commit message"
```
if you choose to run you commit without adding a commit message, git will open a text file in the editor of your choice. Once your message has been written simply save it and close the file.

## Status, Log, and Diff
Status allows you to check you current working directory and the staging area. It will display all unstaged files as red and staged files are green. It also shows which files are currently not being tracked by git.
```
git status
```
git log displays a branches commit history. Running it will provide you with a detailed history and project related information
```
git log
```

## Using The Git Ignore File
If there is certain file(s) or file type(s) you would like git to exclude/ignore, you can create a simple .gitignore file in the projects root folder.
```
# Ignore specific files by adding them
Data.xlx

# ignore all specified file types (WildCard)
*.exe

# Add an exception to the wild card exclusion
!file.a

# Ignore all files in a given folder
supercoolfolder/
```
Here is a list of handy .gitignore files for a variety of purposes
https://github.com/github/gitignore


## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->