---
title: 'Plugin Demo: ipLocate'
slug: iplocate
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
twig_first: true
process:
    twig: true

fields:
    - areaCode
    - city
    - continentCode
    - continentName
    - countryCode
    - countryName
    - currencyCode
    - district
    - dmaCode
    - geonameID
    - gmtOffset
    - isp
    - languages
    - latitude
    - longitude
    - metroCode
    - organization
    - regionCode
    - regionName
    - stateProv
    - timezone
    - zipcode
---

Initial config:

```yaml
sequence:
  - geoplugin
  - dbip
  - freegeoip
  - ipinfo
```

The plugin got the following information. Remember that not all services provide all information. Much of the information is probably blank. This page is not cached.

| Field | Data |
| ----- | ---- |
{% for field in page.header.fields %}
| {{ field }} | {{ attribute(config.plugins.iplocate, field) }} |
{% endfor %}

