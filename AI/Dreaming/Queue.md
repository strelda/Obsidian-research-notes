---
type: dreaming-queue
---
# Dreaming queue

Inputs for the next memory dream. When the owner says "save to memory", add one entry here. Only a dream ([[AI/Skills/memory-dreaming/SKILL|memory-dreaming]]) changes `AI/Memory/`.

## How to add an entry

1. Add your entry at the end of **Inputs**. Do not change any other line of this file.
2. Write what a later session needs and cannot easily get from the project note. Fill only the fields that have content.
3. Link evidence (paths, artifact IDs, commits). Do not paste results, transcripts or secrets.
4. Label each claim: `verified` if you re-ran, recomputed or read the primary data yourself; otherwise `reported (source)`.

```
- [pending] YYYY-MM-DD — agent — project (path of project note)
  - Decisions (with reason):
  - Lessons (what you expected vs what happened):
  - Owner corrections and conventions:
  - Stale or conflicting sources:
  - State change:
  - Evidence:
```

Status: `pending`, `processed: <run ID>` or `failed`. A dream shortens processed entries to one line.

## Inputs
