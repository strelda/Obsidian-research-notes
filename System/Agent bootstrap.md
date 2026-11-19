---
type: agent-bootstrap
ai_access: r
---
# Agent bootstrap

Single canonical text that tells any AI tool where the vault is. Paste it unchanged into: the Claude science project instructions or other platform, the `second-brain` skill description, `AGENTS.md` / `CLAUDE.md` / `GEMINI.md` at the vault root (if used). Keep it short; the rules live in [[Agent rules]], not here.

```text
My second brain is an Obsidian vault at <path-to-your-vault> (e.g., /Users/strelda/Documents/research notes; vault name: "research notes").
When I say "second brain", "my Obsidian", "my notes" or "my memory", it means this vault.
Before any vault work, read README.md, System/Vault map.md and System/Agent rules.md and follow them. They override your defaults.
Use the vault as the only memory for my notes and project facts: do not use your own built-in or project memory for them.
Search with the Obsidian CLI and the access filter described in Agent rules; never grep the whole vault.
If the vault is not accessible, say so and stop; do not save anywhere else.
Never send anything to other people or services.
```
