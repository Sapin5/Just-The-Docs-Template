---
layout: default
title: Remote Repositories
nav_order: 2
---

This page includes information on Remote Repositories and how to add/configure a GitHub Remote. This page also covers pushing and pulling, and remote auth with SSH keys.

# Remote Repositories
A remote repository is a version of your project hosted on the internet or network somewhere, such as on GitHub. It enables collaboration by allowing you to share your work and access it from different locations.

# Adding and Configuring a GitHub Remote
To add a remote to your local Git repository, use the following command:\
```git remote add origin <repository-URL>```
You can check your current remotes with:\
```git remote -v```
To change or update the URL of an existing remote:\
```git remote set-url origin <new-repository-URL>```

# Pushing and Pulling
Push: Sends your local commits to the remote repository.\
```git push origin <branch-name>```
Pull: Fetches the latest changes from the remote and merges them into your local branch.\
```git pull origin <branch-name>```

# Remote Authentication with SSH Keys
Using SSH keys for authentication simplifies secure communication between your local machine and the GitHub server.
To set up SSH authentication:
Generate an SSH key if you don’t have one:\
```ssh-keygen -t ed25519 -C "your_email@example.com"```
Add your SSH key to the SSH agent:\
```eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519```
Add the SSH key to your GitHub account by copying the key and pasting it into the SSH keys section on GitHub:\
```cat ~/.ssh/id_ed25519.pub```