---
layout: default
title: Reset
parent: Undoing
nav_order: 2
---

# When to Use `git reset`

## Best for: Undoing staged changes or revising commit history

`git reset` is a versatile command that can be used to **unstage files**, **rewrite commits**, or **remove changes** entirely. Depending on the options you choose (--soft, --mixed, --hard), it can have different effects.

### **git reset --soft**

- **Use Case**
  You want to undo a commit but keep the changes staged for revision. This allows you to "un-commit" changes but not lose any progress.

-  **When to Use**
If you've made a mistake in your last commit and want to amend or revise it, but still want to keep your changes staged.

-  **Example**
```bash
git reset --soft HEAD~1
```

### **git reset --mixed (default)**
- **Use Case**
  You want to undo a commit and unstage the changes, but keep the changes in your working directory for further editing.

- **When to Use**
  When you’ve committed something prematurely and want to make additional changes before committing again.

- **Example**
```bash
git reset HEAD~1
```
### **git reset --hard**
- **Use Case**
  You want to completely discard all changes, both staged and unstaged, and move your branch pointer back to a specific commit.

- **When to Use**
  Only use `--hard` when you are certain that you don’t need any of the changes after a specific commit. This is a **destructive** option that removes all changes from the working directory and staging area.

- **Example**
```bash
git reset --hard HEAD~1
```

## Key Advantage

`git reset` gives you fine control over staging and commit history. It's perfect for local branches where rewriting history is acceptable.

---