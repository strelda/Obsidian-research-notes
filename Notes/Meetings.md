---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# Meetings

Discussions, sync notes, agendas, and decisions with collaborators.

```base
filters:
  and:
    - 'file.inFolder("Notes")'
    - 'file.name != "Meetings"'
    - 'list(categories).contains("[[Meetings]]")'
views:
  - type: table
    name: "All Meetings"
    order:
      - file.name
      - attendees
      - summary
      - created
```
