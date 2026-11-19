---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# Projects

```base
filters:
  and:
    - file.inFolder("Notes")
    - file.name != "Projects"
    - list(categories).contains("[[Projects]]")
views:
  - type: table
    name: All Projects
    groupBy:
      property: status
      direction: ASC
    order:
      - file.name
      - status
      - created
    sort:
      - property: status
        direction: DESC
      - property: created
        direction: ASC
    columnSize:
      file.name: 468
      note.status: 103

```
