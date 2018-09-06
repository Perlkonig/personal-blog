---
title: 'Google Charts'
slug: google-charts
date: 07-11-2016
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

google-charts: 
  test1: 
    data: 
      - 
        - ID
        - "Life Expectancy"
        - "Fertility Rate"
        - Region
        - Population
      - 
        - CAN
        - 80.66
        - 1.67
        - "North America"
        - 33739900
      - 
        - DEU
        - 79.84
        - 1.36
        - Europe
        - 81902307
      - 
        - DNK
        - 78.6
        - 1.84
        - Europe
        - 5523095
      - 
        - EGY
        - 72.73
        - 2.78
        - "Middle East"
        - 79716203
      - 
        - GBR
        - 80.05
        - 2
        - Europe
        - 61801570
      - 
        - IRN
        - 72.49
        - 1.7
        - "Middle East"
        - 73137148
      - 
        - IRQ
        - 68.09
        - 4.77
        - "Middle East"
        - 31090763
      - 
        - ISR
        - 81.55
        - 2.96
        - "Middle East"
        - 7485600
      - 
        - RUS
        - 68.6
        - 1.54
        - Europe
        - 141850000
      - 
        - USA
        - 78.09
        - 2.05
        - "North America"
        - 307007000
    options: 
      bubble: 
        textStyle: 
          fontSize: 11
      hAxis: 
        title: "Life Expectancy"
      title: "Correlation between life expectancy, fertility rate and population of some world countries (2010)"
      vAxis: 
        title: "Fertility Rate"

imports:
    - 'data.json'
    - 'options.json'
---

## Bare Tag

The data in this case is in the header under

```yaml
google-charts:
  test1:
    data: ...
    options: ...
```

[gchart type=bubble id=test1/]

## Using Import Plugin

Data is loaded into the header using the [Import plugin](https://github.com/Deester4x4jr/grav-plugin-import) and passed in the tag using options.

[gchart type=bar id=test2 data="imports.data" options="imports.options"/]

## Embedded Data

Data and options are passed as a JSON object contained by the tag. Also has the `left` class assigned.

[gchart type=donut id=test3 class="left"]{
    "data": [
        ["Task", "Hours per Day"],
        ["Work", 11],
        ["Eat", 2],
        ["Commute", 2],
        ["Watch TV", 2],
        ["Sleep", 7]
    ],
    "options": {
        "title": "My Daily Activities",
        "pieHole": 0.4
    }
}[/gchart]

