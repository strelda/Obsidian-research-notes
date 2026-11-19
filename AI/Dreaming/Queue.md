---
type: dreaming-queue
last_edited_by: Antigravity
---
# Dreaming queue

Pending inputs for the next manual dream ([[AI/Skills/memory-dreaming/SKILL|memory-dreaming]]). Add only permitted material, never full transcripts, secrets or `ai_access: none/w` content. Status is `pending`, `processed` (with run ID) or `failed` (retry).

A dream remembers only what an entry and the files it links say, so write entries for the future reader, not as a one-line summary. Entry format:

```
- [pending] YYYY-MM-DD — agent — project/topic
  - Decisions (with reason):
  - Lessons / surprises (what failed or differed from expectation):
  - Conventions or owner corrections (how the owner wants things done):
  - Stale or conflicting sources found:
  - State change worth knowing next time:
  - Evidence: [[links]] / paths to logs, reports, commits (do not paste results; link them)
```

Leave a field out if empty. Do not restate what the project note already says. Mark each claim `reported` or `verified`.

## Inputs

- [processed: 2026-11-19_example-init] 2026-11-19 — Antigravity — Example Project (Notes/Example Project.md)
  - Decisions (with reason): gauge choice A selected over B to avoid spurious coordinate singularities in metric tensor calculations (verified 2026-11-19).
  - Lessons / surprises: numerical precision issues near degenerate points require symbolic checks (reported).
  - Conventions or owner corrections: code and raw simulation data kept in external repository; vault keeps synthesis and AI memory (reported).
  - State change worth knowing next time: baseline toy model verified against known analytical limits; simulation pipeline under construction (reported).
  - Evidence: [[Notes/Example Project]].
