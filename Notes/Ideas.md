---
type: category-dashboard
ai_access: r
created: 2026-11-18
---
# Ideas

Sparks, hypotheses, and early research directions to explore or develop.

```base
filters:
  and:
    - 'file.inFolder("Notes")'
    - 'file.name != "Ideas"'
    - 'list(categories).contains("[[Ideas]]")'
views:
  - type: table
    name: "All Ideas"
    order:
      - file.name
      - status
      - summary
      - created
```
