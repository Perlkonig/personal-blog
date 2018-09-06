---
title: 'Plugin Demo: Twig Extensions'
slug: twig-extensions
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
cache_enable: false

---

This page is not cached.

## Intl

| Twig | Result |
| ---- | ------ |
| `'2016-09-29T12:12:12Z'|localizeddate('full', 'full', 'fr')` | `{{ '2016-09-29T12:12:12Z'|localizeddate('full', 'full', 'fr') }}` |
| `1230456.789|localizednumber('decimal', 'default', 'de')` | `{{1230456.789|localizednumber('decimal', 'default', 'de')}}` |
| `1230456.789|localizedcurrency('EUR', 'de')` | `{{1230456.789|localizedcurrency('EUR', 'de')}}` |

## Array

| Twig | Result |
| ---- | ------ |
| `[1,2,3,4,5]|shuffle|join(',')` | `{{[1,2,3,4,5]|shuffle|join(',')}}` |

## Date

| Twig | Result |
| ---- | ------ |
| `'2016-09-29T12:12:12Z'|time_diff` | `{{'2016-09-29T12:12:12Z'|time_diff}}` |


