---
layout: default
title: Git Life Cycle
nav_order: 4
---
# The Git Life Cycle
{: .no_toc }

This page includes information on the Git Life Cycle.

The Git Life Cycle refers to the various stages that files go through in a Git project as they are modified and tracked by the version control system. Understanding these stages is crucial to effectively using Git for version control.

## Working Directory (Untracked/Modified Files)
When you make changes to files in your project, these changes are made in your working directory.
Files in the working directory can be either untracked (not yet added to Git) or modified (tracked but changed since the last commit).

## Staging Area (Staged Files)
The staging area (also called the "index") is where you prepare the changes you want to commit.
You add files to the staging area using:\
```git add <filename>```
Files in this stage are considered "staged" for commit.

## Repository (Committed Files)
Once files are staged, they can be committed to the repository.
A commit is a snapshot of your project’s staged changes at a specific point in time.
To commit the changes in the staging area:\
```git commit -m "Commit message"```
Committed files are now part of the Git history and are safe from further modifications until the next changes are made.

## Git Workflow Overview
1. **Modify**: You edit or create files in the working directory.
2. **Stage**: You move selected changes to the staging area using ```git add```.
3. **Commit**: You save the staged changes to the repository using ```git commit```.
4. **Push**: You send the committed changes to a remote repository (if you're working with one), like GitHub, using ```git push```.

## States of Files in Git
1. **Untracked**: Files that are not yet tracked by Git (not added to the repository).
2. **Modified**: Files that have been changed but not yet staged.
3. **Staged**: Files that have been added to the staging area, ready to be committed.
4. **Committed**: Files that have been saved to the repository with a commit.

## Example Workflow
1. Create or Modify Files:
* You make some changes to your project files.
* These files are now modified or untracked.
2. Stage the Files:\
```git add <filename>```
The files move to the staging area.
3. Commit the Files:\
```git commit -m "Describe your changes"```
The files are saved in the local repository.
4. Push to Remote (Optional):\
```git push origin <branch-name>```
If you're working with a remote repository (like GitHub), you can push your changes to the remote server.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->