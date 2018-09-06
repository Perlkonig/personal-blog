---
title: 'Plugin Demo: Scheduler'
slug: scheduler
date: 22-11-2016
published: true
visible: false
summary:
    enabled: true
    format: short
    size: 128
taxonomy:
    category: []
    tag: [GravDemo]
author: aaron
metadata:
    author: aaron

scheduler:
  active: true
---

The following code block should appear until January 1, 2017.

[scheduler notafter="2016-12-31"]
```
  Can you see me?
```
[/scheduler]

The following code block should not appear until December 1, 2016.

[scheduler notbefore="1 December 2016"]
```
  Can you see me?
```
[/scheduler]


