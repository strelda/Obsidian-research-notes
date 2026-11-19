---
type: vault-map
ai_access: r
---
# Vault map

A short guide to the research brain for its owner and authorized agents. This map describes the vault architecture, not a complete inventory. Privacy labels state intent; configured access controls enforce it. Follow [[Agent rules]] and read [[README]] only if access is permitted and the profile is relevant.

## Access labels

`ai_access` records intended access: `none` means no access, `r` read only, `w` write only, and `rw` read and write. Missing values have intended default `rw`; unrecognized values mean `none`. Only the owner may set or change the property. These labels do not enforce permissions; the connector must implement and test them. A write label does not override approval rules.

## Begin a task

1. Identify the project, idea, memo, or question named by the owner. Begin with its permitted home note in `Notes/` or category dashboard if available.
2. Follow relevant links and use targeted search for supporting material. Load only what helps, but broaden the search when necessary to answer responsibly.
3. At the start of a project task, read `AI/Memory/Index.md` and then only the relevant memory pages. Memory is fallible; verify important claims against their sources.
4. Distinguish the owner's ideas, cited source claims, and AI interpretations. Cite accessible original notes or external sources; report missing or inaccessible context without trying to bypass permissions.
5. Keep agent task plans in `AI/Working/` and suggest changes to human-owned notes in `AI/Proposals/`. Obtain explicit approval for a specific change before modifying human-owned material.

## Vault structure

- **Notes/** — all human-owned notes, project homes, and category dashboards.
  - **Category dashboards:** [[Projects]], [[Ideas]], [[Memos]], [[Sources]], [[People]], [[Meetings]]. Each dashboard embeds an Obsidian Base view filtering notes by linked category.
  - **Project homes:** a project is a note in `Notes/` with the Projects category and property (there is no `Projects/` folder), e.g., [[Example Project]].
- **Daily/** — dated temporal anchors (`YYYY-MM-DD.md`) following Steph Ango's convention. Notes link to dates; daily logs and reviews reside here.
- **Attachments/** — embedded diagrams, local SVGs, images, and files.
- **Templates/** — starter templates for notes, projects, sources, meetings, and daily notes.

## Agent workspace

- **AI/Working/** — temporary plans, active research scratchpads, and handoffs.
- **AI/Proposals/** — AI drafts and suggested changes awaiting owner review and approval.
- **AI/Memory/** — entirely AI-owned memory: `Index.md` (small catalog) and `Topics/<project>/` (small pages by kind). Only a requested dream run changes it; ordinary sessions read it.
- **AI/Dreaming/** — `Queue.md` (pending inputs for the next dream) and `Runs/` (run reports and pre-run snapshots), and `Imports/` (raw source copies kept out of memory).
- **AI/Skills/** — specialized agent workflows (e.g., `obsidian-learning-wiki`, `memory-dreaming`).

## System and policies

- [[Agent rules]] — operating boundaries, approval requirements, and safety protocols.
- [[README]] — owner profile and starting point; marked `r`.
- [[Note properties]] — YAML frontmatter standards and category conventions.
