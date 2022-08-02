---
title: "Git Squash"
date: 2022-08-01T20:47:23+05:30
draft: false
author: "Ashish Shaji"
tags: ["git"]
---
## Git squash
---
### What is a squash?

A squash is a merge commit that merges two or more commits into one.

### Why do I need to squash?

A squash is a way to combine multiple commits into one commit. This is useful when you have a large number of commits that you want to merge into one.

### How do I squash?

To squash commits, use the following commands:

```bash
git rebase -i <commit-id or HEAD~{number}>
```
Example:
```bash
git rebase -i HEAD~2
or
git rebase -i eb8ht3
```

This will open the editor and let you edit the commits.
Replace `pick` with `squash` and save the file.

If the commits have already been pushed to remote, you can use the following command:
```bash
git push origin +branch_name
```
Do not forget to add the (+) sign before the branch name.