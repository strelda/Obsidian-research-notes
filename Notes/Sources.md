---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# Sources

External references, papers, books, articles, preprints, and documentation.

```base
filters:
  and:
    - 'file.inFolder("Notes")'
    - 'file.name != "Sources"'
    - 'list(categories).contains("[[Sources]]")'
views:
  - type: table
    name: "All Sources"
    order:
      - file.name
      - author
      - status
      - summary
      - created
```
