---
type: profile
ai_access: r
---
# Obsidian Research Notes (Collaborative Human-AI Second Brain)

A research knowledge base and second-brain template for [Obsidian](https://obsidian.md), architected for deep human-AI collaboration. It features category dashboards powered by Obsidian Base views, strict agent access-control policies, and an AI memory dreaming system adapted for local vaults.

---

## Architecture Overview

This vault separates human-authored knowledge from the agent workspace while providing structured touchpoints for collaboration:

```
├── .obsidian/         # Obsidian configuration, themes (Things), and recommended plugins
├── Notes/             # Human-owned notes, project homes, and category dashboards
│   ├── Projects.md    # Base view dashboard filtering active/done projects
│   ├── Ideas.md       # Base view dashboard for research hypotheses
│   ├── Memos.md       # Base view dashboard for atomic conceptual notes
│   ├── Sources.md     # Base view dashboard for literature & references
│   ├── People.md      # Base view dashboard for collaborators & researchers
│   ├── Meetings.md    # Base view dashboard for syncs & agendas
│   └── Example Project.md # Sample project note demonstrating structure
├── Daily/             # Temporal anchors (YYYY-MM-DD.md) following Steph Ango's convention
├── Attachments/       # Diagrams, local figures, PDFs, and assets
├── Templates/         # Reusable frontmatter templates (Daily, Idea, Meeting, Note, Person, Project, AI session log)
├── System/            # Vault policies and agent configuration
│   ├── Agent bootstrap.md # Canonical prompt pointing AI models to this vault
│   ├── Agent rules.md     # Operating boundaries, privacy labels, and write permissions
│   ├── Vault map.md       # High-level architecture guide for navigation
│   └── Note properties.md # Frontmatter specifications and category rules
└── AI/                # Dedicated AI workspace
    ├── Memory/        # Distilled, persistent AI memory
    │   ├── Index.md   # Catalog loaded by AI agents at task start (<100 lines)
    │   └── Topics/    # Granular project memory pages (State, Decisions, Conventions, Lessons, Open questions)
    ├── Dreaming/      # Memory consolidation pipeline
    │   ├── Queue.md   # Pending inputs awaiting manual memory consolidation
    │   ├── Runs/      # Run reports and pre-run snapshots
    │   └── Imports/   # Raw external source copies kept out of compact memory
    ├── Skills/        # Specialized agent workflow instructions (memory-dreaming, obsidian-learning-wiki)
    ├── Working/       # Task plans, scratchpads, and execution logs
    └── Proposals/     # Drafts and suggested changes awaiting user review
```

---

## Core Principles

1. **Human Ownership & Boundary Enforcement**: Human notes in `Notes/`, `Daily/`, and `System/` require explicit user approval before any AI edits. AI agents propose changes via `AI/Proposals/` or work within `AI/Working/`.
2. **Granular Access Control**: Frontmatter property `ai_access` (`rw`, `r`, `w`, `none`) dictates read/write permissions per note.
3. **AI Memory Dreaming**: Based on Anthropic's memory dreaming architecture adapted for local file systems. Instead of bloating agent context with entire chat transcripts or raw notes, key decisions, verified facts, conventions, and surprises are queued in `AI/Dreaming/Queue.md` and consolidated into `AI/Memory/Topics/` during requested dream runs.
4. **Base View Dashboards**: Category pages in `Notes/` embed Obsidian Base views that dynamically query and group notes by category (`[[Projects]]`, `[[Ideas]]`, `[[Memos]]`, `[[Sources]]`, `[[People]]`, `[[Meetings]]`).

---

# Me (User Profile & Agent Starting Point)

This section contains the profile information and instructions read by AI assistants at the start of vault sessions.

## Research and knowledge

- This folder contains a personal research knowledge base in Obsidian to manage several research directions and projects.
- Notes follow category-based structure in `Notes/` (using categories like `[[Projects]]`, `[[Ideas]]`, `[[Memos]]`, `[[Sources]]`, `[[People]]`, `[[Meetings]]`).
- I value connections between ideas, research, sources, and projects, and want a structure that remains manageable over time.

## Working with AI

- My notes and ideas are the core of the system. Agents can propose changes to my notes and obtain my explicit approval before making them.
- AI has its own working area, proposals, and compact memory. A dreaming process should consolidate memory from permitted material and track what has been processed.
- I care about privacy, portability and open-source.
- Project connections to GitHub, local folders, reMarkable, Apple Notes, Zotero, and other resources are optional. A link does not grant access, but it helps steer that way (e.g. search the Zotero folder for articles or save new ones to the appropriate folder), or suggest to look at other locations for missed notes.
- You are forbidden from sending anything to other people or platforms without explicit approval; you collaborate ONLY with me.

## Navigation and context

- Start with [[Vault map]] and [[Agent rules]].
- Prefer a relevant project or research map and linked sources over reading the whole vault. Keep project context and AI memory concise, but retrieve more when a question needs it.
- Distinguish my own ideas and decisions from source claims, AI interpretations, and uncertain memory. Cite original sources when possible. Always retain moral standards of attributing credit for ideas and work to others. This regards code, articles, knowledge based on discussions with collaborators, etc.

## Additional context

Add research interests, preferred working styles, and other details here when ready.
