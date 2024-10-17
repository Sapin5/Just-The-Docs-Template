---
layout: default
title: Checkout
parent: Undoing
nav_order: 1
---

# When to Use `git checkout`

## Best for: Undoing changes to individual files (not yet staged)

`git checkout` is ideal when you want to undo changes made to a **specific file** in your working directory that hasn't been staged yet. It allows you to discard changes in a file and revert it to the last committed state.

- **Use Case**:  
  You’ve modified a file but haven’t staged it yet with `git add`. Now, you realize you don’t want those changes and wish to discard them:

```bash
git checkout -- <file>
```
## Key Advantage

Only the specified file is affected, and no commits or other changes are impacted.

## When to Use

Use `git checkout` if you only want to discard changes in your working directory without affecting the staging area or commit history.