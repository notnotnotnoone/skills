# notnotnotnoone/skills

A collection of portable, production-tested AI agent skills adhering to the portable Agent Skills specification.

## Included Skills

### 1. `system-content-segregation-transfer`
**Folder:** [`skills/system-content-segregation-transfer/`](skills/system-content-segregation-transfer/)  
**Purpose:** Deep forensic filesystem audit, LLM swarm classification, non-destructive directory junction staging, and automated data transfer & purge for separating mixed user data across Windows computers.
- **Key Concepts:**
  - Top-down tree audit with hierarchical branch pruning.
  - LLM swarm inspection of file internals (embedded Word/PDF metadata, SQLite databases, and browser profiles) instead of fragile filename regex rules.
  - Zero-touch staging via native Windows Directory Junctions (`mklink /J`) and `.lnk` shortcuts.
  - Two-phase guarded transfer and irreversible purge runner.

---

### 2. `evaluate-app-idea`
**Folder:** [`skills/evaluate-app-idea/`](skills/evaluate-app-idea/)  
**Purpose:** A skeptical, research-driven skill for deciding whether a software or app idea deserves development across 32 rigorous criteria.

---

## Installation & Usage

### Compatible Agent Systems (Codex, Antigravity, Claude Desktop, Cursor)

Clone or copy the individual skill folder into your agent's skills directory:

- **Project-level:** `.agents/skills/<skill-name>/`
- **User-level:**
  - Codex: `$CODEX_HOME/skills/<skill-name>/`
  - Antigravity / Gemini: `~/.gemini/config/skills/<skill-name>/`
  - Claude: `~/.claude/skills/<skill-name>/`

Each skill directory contains a self-contained `SKILL.md` with standard YAML frontmatter.
