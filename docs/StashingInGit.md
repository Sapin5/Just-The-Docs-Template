---
layout: default
title:  What is Stashing in git?
nav_order: 6
---

## What is _Stashing_ in Git?

Stashing is a way of hiding away changes made to a repository either to be added to a later commit, or brought to another branch. The stash functions like stacking papers, where the most recently added items are the ones that will be removed first.
To put a set of changes on the stash, you can use the terminal command `git stash push`.
To retrieve a set of changes, you can use the terminal command `git stash pop` or alternatively `git stash show` to preview the changes, followed by `git stash apply` to apply the previewed changes onto the current branch.
You can view your current stash stack by using `git stash list`, and create a new branch based on stashed changes by using `git stash branch [branch name]`. To remove stashed changes from your stack without applying them anywhere, the command `git stash drop [stash name]` can be used.

The `stash push` command can be used alongside several optional parameters such as:
 - `-a`/`--all`: any ignored or untracked files in the repository are added to the stash and removed from the working directory.
 - `-u`/`--include-untracked`: includes untracked files, which are then removed from the working directory.
 - `-s`/`--staged`: only pushes staged filed to the stash. Basically works like a commit to the stash instead of the current branch.
 - `--patch`: pick and chose individual changes to be stashed within the working directory.
