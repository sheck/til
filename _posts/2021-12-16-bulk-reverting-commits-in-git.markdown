---
title: Bulk reverting commits in Git
date: 2021-12-16 05:47:00 Z
---

To bulk revert a bunch of commits in Git (like, to [redo your personal site from scratch](https://github.com/sheck/sheck.github.io/commit/ce76eb31daa3568cee7128c87a8d6eb1ecb98964)) do this:

```shell
$ git revert -n <very first bad sha>^..HEAD
$ git commit
```

(the `-n` flag will squash the revert without committing, omitting it means you have to commit a revert for every. single. commit.)