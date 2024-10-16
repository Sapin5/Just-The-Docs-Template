---
layout: default
title: Clean
parent: Undoing
nav_order: 4
---

# When to Use `git clean`

## Best for: Undoing untracked file changes

`git clean` is the command to use when you want to **remove untracked files** from your working directory. These files might be temporary, generated by build processes, or files that you created but decided not to keep.

- **Use Case**
 Your working directory has become cluttered with untracked files, and you want to clean up your workspace:

```bash
git clean -f
```
## Key Advantage

It removes files that Git isn’t tracking, leaving the tracked files and changes untouched.

## When to Use
  
Use `git clean` when you need to clean up untracked files, such as build artifacts, from your working directory. Be cautious, as this action is irreversible through Git.

---