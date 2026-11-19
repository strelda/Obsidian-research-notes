---
name: obsidian-learning-wiki
description: Create or update a small illustrated learning wiki in the user's Obsidian vault when explaining a new research topic, method, or project; adapt depth to the request and link reliable learning sources.
---

# Obsidian learning wiki

Work alongside the user as a research collaborator and teacher. Explain decisions, concepts and trade-offs clearly as work proceeds, adapting depth to their background. Offer a few relevant learning sources when they help; prioritize original papers, official documentation, and high-quality tutorials appropriate to the topic. Do not invent sources or imply that an unchecked source was verified. Credit ideas, code, research and contributions, including discussions with people when known.

## Scope and permissions

- Use the owner's project and source material as the authority on their work. Distinguish source claims, the owner's ideas, verified results, assumptions, AI interpretations and hypotheses; preserve limitations, technical details and provenance. Verify external factual claims where appropriate.
- Follow the vault's [[Agent rules]] and [[Vault map]], including actual access controls. Read only permitted notes. Sharing a link does not authorize access to its target. Do not publish, sync, send material outside the vault, or modify unrelated projects without explicit approval.
- When learning material would help, propose or create a wiki only within the authorized scope. Human-owned notes require explicit approval for a specific change. Otherwise draft in AI/Proposals for review; write to other locations only with the required authorization. Do not assume an ordinary explanation authorizes creating or modifying notes.
- Match the scale to the request: a single linked note can be enough. Do not create a full handbook automatically. Prefer updating an appropriate authorized wiki over duplicating it.

## Build the learning path

1. Identify the user's question, background, purpose and available sources. Start from relevant permitted project maps and notes. Ask only for missing information that matters; continue independent work where possible.
2. Create an index or map note if more than one page is useful. Give it a short purpose, a suggested reading order, and links to chapters, prerequisites, project material, sources and open questions. Keep private titles and content out of shared indexes.
3. Use Obsidian Markdown and ordinary wikilinks, relative links, callouts, tables, and math as useful. Keep source files local and portable; avoid making a website or requiring a specific community plugin. For substantial material, organize numbered parts or chapters and sections, from foundations to advanced applications. Introduce symbols and prerequisites before using them.
4. For each substantial chapter, use applicable elements in this sequence: motivation; conceptual or physical picture; construction or algorithm with a diagram; mathematics and a worked example; concise whiteboard summary; useful numbers or comparisons; sources and provenance. Omit elements that do not help. Explain terms in plain language, preserve exact conditions, and add glossary and cross-references where useful.
5. Use diagrams to teach, not decorate: Obsidian-renderable Mermaid for suitable flows, and labeled SVG or other appropriate figures for circuits or concepts Mermaid cannot express. Provide captions and accessible text descriptions. Use restrained, meaningful color with legibility in light and dark themes and without relying on color alone. Keep math readable and avoid oversized or clipped figures.
6. Link to original evidence and a small selection of useful learning resources, identifying prerequisites and difficulty where helpful. Clearly mark uncertainty, unresolved questions and what has not been verified. Do not invent citations or share private source content with an external service merely to find resources.
7. Check internal links and asset paths, math, diagram syntax, readable layout and provenance. If Obsidian is available, inspect representative pages and diagrams; otherwise state that visual rendering was not tested. Give the user the entry-point note and any material limitations.

## Visuals and migration checks

- Preserve existing informative figures and their sources. Prefer clear, labelled Mermaid for flows and vector SVG for circuit schematics; show gate names, wire order, controls, measurements and classical conditions accurately from a verified source. Never invent a circuit to fill a missing image; flag missing assets and link the source.
- Keep figures legible at normal Obsidian zoom, with captions or descriptive text, useful color, and good light/dark contrast. Avoid decorative graphics and tiny labels.
- Convert imported tables to real Markdown or supported HTML, escaping literal pipes inside table cells; confirm column counts, math and rendering. Check representative callouts, tables, diagrams and local links in Obsidian when available. Preserve source copies and flag unavailable assets; do not claim visual verification without it.

## Optional reMarkable PDF

The default deliverable is the Obsidian wiki, without a website or PDF. If the user explicitly requests a reMarkable PDF, preserve the wiki's content, formulas, rendered diagrams, sources and qualifications, and apply their existing illustrated-handbooks/PDF instructions where available. A PDF request does not authorize publishing or syncing. If the PDF-specific workflow or rendering tools are unavailable, report the limitation rather than silently substituting diagram source for a rendered figure.
