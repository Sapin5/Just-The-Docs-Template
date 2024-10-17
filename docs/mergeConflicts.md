---
layout: default
title: Merge Conflicts
nav_order: 3
---

# What is a merge conflict?

Merge conflicts occur when Git can't automatically merge two branches.
When a merge conflict happens, Git will alert you in the terminal and mark the areas of
conflict in the file.

---

## Git's Markup of Conflicted Files
Git uses special markers to indicate the start and end of the conflicted area:
```plaintext
<<<<<<< HEAD
```
and: 
```plaintext
======= 
```
as the separator between the changes in the current and the other branch.
```plaintext
>>>>>>> branch-name
```
shows the end of the changes in the other branch.

---

## How do we resolve merge conflicts?
To resolve a merge conflict:
1. Edit the file to fix the conflicting changes. Be sure to remove the conflict markers.
2. Add the file to the staging area with git add .
3. Commit the fix with git commit .

Only the specified file is affected, and no commits or other changes are impacted.

---