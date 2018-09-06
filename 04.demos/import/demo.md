---
title: 'Plugin Demo: Import'
slug: import
date: 30-10-2016
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

imports:
    - 'file1.yaml'
    - 'user://data/file2.json'
    - 'user://data/scratch/file3.json'

---

#Header

```yaml
imports:
    - 'file1.yaml'
    - 'user://data/file2.json'
    - 'user://data/scratch/file3.json'
```

## File1

### Input

```yaml
var1: val1
var2:
  - var2a: val2a
    var2b: val2b
```

### Output

Via `page.header.imports.file1|json_encode(constant('JSON_PRETTY_PRINT'))`:

<pre>
{{ page.header.imports.file1|json_encode(constant('JSON_PRETTY_PRINT')) }}
</pre>

## File 2

### Input

```json
{
  "var1": "val1",
  "var2": [{
    "var2a": "val2a",
    "var2b": "val2b"
  }]
}
```

### Output

Via `page.header.imports.file2|json_encode(constant('JSON_PRETTY_PRINT'))`:

<pre>
{{ page.header.imports.file2|json_encode(constant('JSON_PRETTY_PRINT')) }}
</pre>

## File 3

### Input

```json
{
  "var1": "val1",
  "var2": [{
    "var2a": "val2a",
    "var2b": "val2b"
  }]
}
```

### Output

Via `page.header.imports.file3|json_encode(constant('JSON_PRETTY_PRINT'))`:

<pre>
{{ page.header.imports.file3|json_encode(constant('JSON_PRETTY_PRINT')) }}
</pre>


