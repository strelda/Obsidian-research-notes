# Note properties

The research brain follows Steph Ango's category-based structure. Reusable human notes live in `Notes/` and use YAML frontmatter properties for categorization, status, and agent access.

## Standard properties

- **categories**: a list of wikilinks to category pages, following Steph Ango's pluralization rule (e.g., `["[[Projects]]", "[[Quantum computing]]"]`). Core categories:
  - `[[Projects]]` — reserved STRICTLY for the topmost pages of projects (e.g., [[Example Project]]). Never assign `[[Projects]]` to sub-pages, chapters, documentation, wiki notes, or task lists within a project.
  - `[[Ideas]]` — early hypotheses, sparks, or research directions to develop.
  - `[[Memos]]` — conceptual notes, observations, and reusable knowledge.
  - `[[Sources]]` — literature, preprints, books, papers, or documentation.
  - `[[People]]` — collaborators, researchers, and contacts.
  - `[[Meetings]]` — sync notes, agendas, and discussions.
- **status**: note or project lifecycle status:
  - `active` — currently in progress.
  - `waiting` — blocked or waiting on external dependencies (collaborator, grant decision, reviewer).
  - `TBD` — to be determined / pending definition or scoping.
  - `done` — finished / completed.
  - `archived` — deprecated or put on hold indefinitely.
- **ai_access**: `none`, `r`, `w`, or `rw`. The owner controls this property. The template defaults to `rw`, matching the vault policy; these labels state intent and are enforced by connectors.
- **summary**: a concise one-sentence description for fast navigation and Base views.
- **created**: creation date in `YYYY-MM-DD` format.
- **last_edited_by**: optional editor identifier (`me`, `Codex`, `Claude`, etc.).
- **source**: optional link or citation to original external material (URL, DOI, Notion ID).
