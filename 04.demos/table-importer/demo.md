---
title: 'Plugin Demo: Table Importer'
slug: table-importer
date: 06-11-2016
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
---

## JSON (with caption)

```json
[
  ["Col1", "Col2", "Col3"],
  ["Val1", "Val2", "Val3"],
  ["Val4", "Val5", "Val6"],
  ["Val7", "Val8", "Val9"]
]
```

[ti file=test-json.json caption="Caption: Simple JSON example"/]

## JSON from `user/data` folder

```json
[
  ["Col1", "Col2", "Col3"],
  ["Val1", "Val2", "Val3"],
  ["Val4", "Val5", "Val6"],
  ["Val7", "Val8", "Val9"]
]
```

[ti file="data:test-json.json"/]

## YAML

```yaml
-
  - Col1
  - Col2
  - Col3
-
  - Val1
  - Val2
  - Val3
-
  - Val4
  - Val5
  - Val6
-
  - Val7
  - Val8
  - Val9
```

[ti=test-yaml.yaml/]

## CSV

Example without headers.

```csv
Col1,Col2,Col3
Val1,Val2,Val3
Val4,Val5,Val6
Val7,Val8,Val9
```

[ti file=test-csv.csv header=false/]
