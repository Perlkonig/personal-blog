---
title: 'Plugin Demo: Twig Jasny Array'
slug: twig-jasny-array
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

twig_first: true
process:
    twig: true

data:
    array1: 
        - 1
        - 2
        - 3
        - 4
        - 5
    array2:
        one: 1
        two: 2
        three: 3
        four: 4
        five: 5

---

Seed data:

```yaml
data:
    array1: 
        - 1
        - 2
        - 3
        - 4
        - 5
    array2:
        one: 1
        two: 2
        three: 3
        four: 4
        five: 5
```

| Twig | Results |
| ---- | ------- |
| `data.array1 | sum` | `{{ page.header.data.array1 | sum }}` |
| `data.array1 | product` | `{{ page.header.data.array1 | product }}` |
| `data.array2 | values | sum` | `{{ page.header.data.array2 | values | sum }}` |
| `data.array2 | html_attr` | `{{ page.header.data.array2 | html_attr }}` |

