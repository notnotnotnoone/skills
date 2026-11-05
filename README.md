# App Idea Review

A skeptical, research-driven skill for deciding whether a software or app idea deserves development.

## Install

This repository follows the portable Agent Skills folder convention.

### Codex

Clone or download this repository, then place the skill folder at either:

- Project-level: .agents/skills/evaluate-app-idea/
- User-level: $CODEX_HOME/skills/evaluate-app-idea/

The resulting path must contain SKILL.md, for example:

.agents/skills/evaluate-app-idea/SKILL.md

Restart or refresh the agent session if the skill is not detected.

### Other compatible agents

Use the same folder structure in the agent's documented skills directory. Skill discovery and invocation syntax vary by product. The skill's name is evaluate-app-idea; a compatible agent may expose it as $evaluate-app-idea or through its own skill picker.

## Use

Invoke the skill with a pitch, for example:

$evaluate-app-idea I want to build a Windows app that...

It performs a quick rejection screen, researches alternatives, evaluates all 32 criteria, and uses independent sub-agent reviews only when the idea survives initial screening and the environment supports sub-agents.

## Design notes

- The original development transcript explicitly listed 30 criteria in a numbered table.
- Two additional cross-cutting rules were added later: total expected benefit must justify both user adoption effort and developer effort; and trivial built-in actions must be checked before proposing automation.
- The exported transcript does not define a numeric weighting formula. The skill therefore uses categorical criterion statuses and four verdicts rather than inventing a score.
- Typer/Completionist and Flexrouter are included as calibration examples, not predetermined endorsements or rejections.

## Portability

The skill is plain Markdown with YAML frontmatter and no account-specific dependencies. Research tools, sub-agents, and web access depend on the host agent. When a capability is unavailable, the agent must disclose that limitation rather than pretend it ran.
