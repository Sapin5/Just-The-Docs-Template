---
layout: default
title: Revert
parent: Undoing
nav_order: 3
---

# When to Use `git revert`

## Best for: Undoing changes in a safe, non-destructive way

`git revert` is the preferred method when you need to undo changes in a public or shared branch. It creates a new commit that reverses the changes introduced by a previous commit, leaving the original commit history intact.

- **Use Case** 
  You’ve made a mistake in a previous commit that’s already been pushed to a shared branch (like `main`), and you need to undo the changes without rewriting history:
```bash
git revert <commit>
```
## Key Advantage 

`git revert` is non-destructive and safe to use in shared repositories because it doesn’t rewrite commit history; it simply adds a new commit that negates a previous one.

## Key Advantage 

Use `git revert` when you need to safely undo a commit in a public branch or when you want to ensure that your repository's history remains intact.

---