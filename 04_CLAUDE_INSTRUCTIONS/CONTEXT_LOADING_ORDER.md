# CONTEXT LOADING ORDER

## Version: 2.0
## Date: 2026-06-17
## Updated: Token-efficiency revision

---

## Purpose

GitHub Context OS is a **token-efficiency layer**, not a full-context reload system.
Load only the minimum context required for the task.
Do not run the full sequence as a ritual.

---

## 1. Default Minimal Load

Run these 4 files at the start of every session:

```
STEP 1  →  00_CONTEXT_CORE/SESSION_INIT.md
           (Session startup checklist)

STEP 2  →  04_CLAUDE_INSTRUCTIONS/SYSTEM_PROMPT.md
           (Active operating identity and rules)

STEP 3  →  01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md
           (What happened last session)

STEP 4  →  02_OPERATIONAL_FILES/ACTIVE_TASKS.md
           (Current task state)
```

These 4 files are the complete default load. Stop here unless a conditional trigger applies.

---

## 2. Conditional Load

Load additional files only when a specific trigger arises. Do not pre-load.

| File | Load Only When |
|------|----------------|
| `00_CONTEXT_CORE/CONTEXT_OS_MANIFEST.md` | Claude needs the full repo structure |
| `00_CONTEXT_CORE/MASTER_INSTRUCTION_SET.md` | Operating rules are unclear or behaviour drifts |
| `04_CLAUDE_INSTRUCTIONS/BEHAVIOR_RULES.md` | Tone or execution behaviour needs correction |
| `01_MEMORY_LAYERS/LONG_TERM_MEMORY.md` | After context loss or a major reset |
| `02_OPERATIONAL_FILES/PROJECT_REGISTRY.md` | Active project is unclear |
| `02_OPERATIONAL_FILES/ASSET_INDEX.md` | Locating or checking an asset |
| `03_PROTOCOL_ENGINE/RESET_PROTOCOL.md` | During a reset |
| `03_PROTOCOL_ENGINE/ESCALATION_PROTOCOL.md` | When blocked and cannot proceed |
| `03_PROTOCOL_ENGINE/HANDOFF_PROTOCOL.md` | At session close |
| `05_ARCHIVE/CHANGELOG.md` | During audit or history review |

---

## 3. Boundary Note

> **GitHub Context OS exists to reduce token usage by loading only the minimum context required for the task. It must not become a full-context ritual. Google Drive remains the source of truth for full Coffee Performance files.**
>
> ---
>
> ## Loading Confirmation
>
> After completing the default minimal load, Claude should state:
> > "Minimal context loaded. [4 files]. Active tasks reviewed. Ready."
> >
> > Only if conditional files were also loaded:
> > > "Context loaded. [N] files. Triggered by: [reason]. Ready."
> > >
> > > ---
> > > _Keep this file updated if trigger conditions change. Version history in 05_ARCHIVE/CHANGELOG.md_
