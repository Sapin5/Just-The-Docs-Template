---
layout: default
title:  What is Stashing in git?
nav_order: 5
---

## What are _Tags_ in Git?

Git tags are a way of labelling specific commits. This can be used for organization and documentation, such as marking specific versions of your repository with descriptive labels (example: `v0.12.4`). There are two kinds of tag, a lightweight tag, which is just a label, and an anotated tag, which contains metadata such as who added the tag, when it was added, and an associated message.
To add a tag to a commit, you can use the terminal command `git tag [tag name] [commit hash]`. If the commit hash is left out, the tag will be applied to the head of the repository. To create an anotated tag instead of a lightweight one, the `-a` parameter can be added between `tag` and `[tag name]`. Note that if the `-m` parameter as well as a message is not provided, a text editor will be opened so you can provide the message at that time.
Tags can also be used in place of the hash for the commit they are associated with in various git commands that can take in commit hashes such as `git checkout`. By default they are not pushed to remotes with the `git push` command, but can either be passed explicitly (example: `git push origin v0.12.4`) or pushed by adding the `--tags` argument to a push command.
