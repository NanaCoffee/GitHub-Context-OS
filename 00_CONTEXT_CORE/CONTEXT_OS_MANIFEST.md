# CONTEXT OS MANIFEST

## Version: 1.0
## Date: 2026-06-17
## Owner: NanaCoffee

---

## Purpose
The GitHub Context OS is a structured system for managing Claude AI context, memory layers, operational files, and protocols across all projects.

## Core Directories

| Folder | Purpose |
|--------|--------|
| `00_CONTEXT_CORE/` | Master instructions, manifest, session init |
| `01_MEMORY_LAYERS/` | Long-term, short-term, and working memory |
| `02_OPERATIONAL_FILES/` | Active tasks, project registry, asset index |
| `03_PROTOCOL_ENGINE/` | Reset, escalation, and handoff protocols |
| `04_CLAUDE_INSTRUCTIONS/` | System prompts, behavior rules, loading order |
| `05_ARCHIVE/` | Changelog and historical records |

## Loading Order
1. SESSION_INIT.md
2. MASTER_INSTRUCTION_SET.md
3. LONG_TERM_MEMORY.md
4. SHORT_TERM_CONTEXT.md
5. ACTIVE_TASKS.md

## Governance
- All files use Markdown format
- Updates logged in `05_ARCHIVE/CHANGELOG.md`
- Version controlled via Git (main branch)
