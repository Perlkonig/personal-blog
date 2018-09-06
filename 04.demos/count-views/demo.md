---
title: 'Count Views'
slug: count-views
date: 08-11-2016
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

cache_enabled: false
twig_first: true
process:
    twig: true
---

## Most Popular Blog Posts

{% if viewcounts is defined %}
{% for route,views in viewcounts|sort|reverse|slice(0,20) %}
    {% set p = page.find(route) %}

* [{{ p.title }}]({{ route }}) ({{views}})

{% endfor %}
{% endif %}

