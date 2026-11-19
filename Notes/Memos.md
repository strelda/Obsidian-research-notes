---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# Memos

Observations, concepts, atomic notes, and knowledge to recall or reuse across projects.

```base
filters:
  and:
    - 'file.inFolder("Notes")'
    - 'file.name != "Memos"'
    - 'list(categories).contains("[[Memos]]")'
views:
  - type: table
    name: "All Memos"
    order:
      - file.name
      - status
      - summary
      - created
```
