# core Plugin

**Version:** 0.1.0 | **Author:** TBD
**Purpose:** Universal agent behavior, documentation standards, and shared tooling across all teams.

## Overview

Provides universal behavior and documentation standards, plus shared utility commands and shared assets used by all other plugins. Install this plugin in every workspace to enforce baseline conduct/documentation rules and provide shared utilities for note capture and documentation generation.

This plugin maps to all SDLC phases (Cross-phase) and is utilized by everyone, including PM, Analyst, Developer, Architect, and QA roles. It establishes the groundwork for interactions with AI agents, ensuring high-quality outputs, uniform conventions, and consistent documentation practices.

## SDLC Pipeline Context
- **Inputs:** Existing project documentation, forensic deep-dive reports, and solution overviews.
- **Outputs:** Utility documentation artifacts, structured session notes (`docs/notes/`), generated plugin documentation (`README.md`), solution overviews (`docs/[solution-name]-solution-overview.md`), and how-to guides (`docs/[solution-name]-how-to.md`).

## Dependencies & Integrations
- **MCP Servers:** MS Learn Docs, Atlassian
- **External CLI/Tools:** None specified

## Included Assets

### 💻 Commands
| Command | Description |
| ------- | ----------- |
| `/capture-notes` | Capture structured session notes and actionable follow-ups. |
| `/generate-how-to-guide` | Create practical how-to documentation for implemented workflows. |
| `/generate-plugin-doc` | Generate comprehensive documentation for a specific SDLC plugin based on its current directory contents and manifest. |
| `/generate-solution-overview` | Produce concise solution overview documentation from project context. |

### 🧠 Skills
| Skill | Description |
| ----- | ----------- |
| `plugin-scaffold-governance` | Create or validate repository plugin scaffolds against the marketplace baseline. Use when a repository maintainer needs to scaffold a plugin, validate plugins, or repair template drift. |

### 📏 Rules Enforced
| Rule | What it enforces |
| ---- | ---------------- |
| `conduct.mdc` | Baseline conduct and review posture for all work. Apply when assessing quality, security, assumptions, and documentation placement. |
| `documentation-standards.mdc` | Documentation baseline for markdown, README, and XML-style docs. Apply when authoring or reviewing user-facing documentation. |
| `git-conventions.mdc` | Apply shared git, changelog, and pull request conventions during repository updates and delivery work. |
