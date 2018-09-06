---
title: 'Plugin Demo: Pubmed'
slug: pubmed
date: 30-09-2016
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

cache_enable: false

---

Initial config:

```yaml
formats:
  short: "[authors_short] [journal] [volume] [pages] [date]"
  long: '<a href="https://www.ncbi.nlm.nih.gov/pubmed/[uid raw]">[title]</a><br>[authors_long] [journal] [volume] [pages] [date]'
  author_sep: ", "  # string that is inserted between list of authors when using [authors_long]
```

Publication number being searched: `9039911`. Click the "View Original Source" link for details.

This page is not cached.

## Short

[pubmed type=short ids=9039911]

## Long

[pubmed type=long ids=9039911]

## Summary

[pubmed type=summary ids=9039911]
