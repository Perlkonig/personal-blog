---
title: 'Plugin Demo: Backlinks'
slug: backlinks
date: 16-11-2016
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
twig_first: true
process:
    twig: true
---

## Pages referenced more than twice

{% set counts = [] %}
{% for key in backlinks|keys %}
    {% set counts = counts|merge({(key): backlinks[key]|count}) %}
{% endfor %}

| Page | Time Referenced |
| ---- | ---- |
{% for route, num in counts|sort|reverse if num>2 %}
    {% set page = page.find(route) %}
| [{{ page.title }}]({{route}}) | {{num}} |
{% endfor %}
