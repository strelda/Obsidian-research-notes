---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# People

Collaborators, researchers, authors, and contacts with shared context and discussions.

```base
filters:
  and:
    - 'file.inFolder("Notes")'
    - 'file.name != "People"'
    - 'list(categories).contains("[[People]]")'
views:
  - type: table
    name: "All People"
    order:
      - file.name
      - summary
      - created
```
