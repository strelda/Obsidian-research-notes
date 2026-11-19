---
type: ai-memory-lessons
summary: Surprises, failure modes, and practical lessons learned during the example project.
created: 2026-11-19
last_verified: 2026-11-19
last_edited_by: Antigravity
source: "[[Notes/Example Project]]"
---
# Example Project: lessons

- Beware of floating-point precision loss when evaluating small eigenvalue differences near degenerate points; use quadruple precision or exact symbolic diagonalisation where needed.
