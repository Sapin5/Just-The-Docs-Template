---
layout: default
title: When to use different strategies
parent: Undoing
nav_order: 5
---

# Choosing the Right Strategy

## Use `git checkout` if you want to undo changes in individual files that haven’t been staged yet. It’s non-destructive and affects only the working directory.

## Use `git revert` if you need to undo a commit in a shared or public branch without rewriting history. It’s the safest method for undoing commits in collaborative environments.

## Use `git reset` if you need to undo staged changes or adjust commit history on a local branch. It offers flexibility but be careful with the `--hard` option, as it’s destructive.

## Use `git clean` if you want to remove untracked files from your working directory, cleaning up temporary or unwanted files that aren’t part of the repository.

---