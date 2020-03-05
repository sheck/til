---
title: Searching for files that contain X _and_ Y
date: 2020-03-05 23:48:00 Z
---

If you're trying to find files that contain two distinct strings, you can use ag (or grep) and unix to do it. So to find all files that have `spec_helper` AND `stub_request`:

```shell
$ ag -l spec_helper | xargs ag stub_request
```