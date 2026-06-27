# SESSION INIT

## Version: 2.0
## Date: 2026-06-17
## Updated: Aligned with Context Loading Order v2.0

---

## Default Mode: OPERATION

Operate from the active task, not the full history.
Load only the minimum context required. Do not run the full sequence as a ritual.

---

## Session Startup — Default Minimal Load

Run these 4 files only at the start of every session:

- [ ] **STEP 1** — Read `00_CONTEXT_CORE/SESSION_INIT.md` _(this file)_
- [ ] - [ ] **STEP 2** — Read `04_CLAUDE_INSTRUCTIONS/SYSTEM_PROMPT.md`
- [ ] - [ ] **STEP 3** — Read `01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md`
- [ ] - [ ] **STEP 4** — Read `02_OPERATIONAL_FILES/ACTIVE_TASKS.md`

- [ ] Stop here. Do not load additional files unless a conditional trigger applies.

- [ ] ---

- [ ] ## Conditional Files — Load Only When Triggered

- [ ] Do not pre-load. Load only when the specific need arises.

- [ ] | File | Load Only When |
- [ ] |------|----------------|
- [ ] | `CONTEXT_OS_MANIFEST.md` | Full repo structure is needed |
- [ ] | `MASTER_INSTRUCTION_SET.md` | Operating rules are unclear or behaviour drifts |
- [ ] | `BEHAVIOR_RULES.md` | Tone or execution needs correction |
- [ ] | `LONG_TERM_MEMORY.md` | After context loss or major reset |
- [ ] | `PROJECT_REGISTRY.md` | Active project is unclear |
- [ ] | `ASSET_INDEX.md` | Locating or checking an asset |
- [ ] | `RESET_PROTOCOL.md` | During a reset |
- [ ] | `ESCALATION_PROTOCOL.md` | When blocked and unable to proceed |
- [ ] | `HANDOFF_PROTOCOL.md` | At session close |
- [ ] | `CHANGELOG.md` | During audit or history review |

- [ ] ---

- [ ] ## Session Declaration

- [ ] After completing the default minimal load, state:
- [ ] > "Minimal context loaded. [4 files]. Active tasks reviewed. Ready."

- [ ] If conditional files were also loaded:
- [ ] > "Context loaded. [N] files. Triggered by: [reason]. Ready."

- [ ] ---

- [ ] ## Session Notes

- [ ] Date: ___________
- [ ] Project: ___________
- [ ] Session Goal: ___________
- [ ] Known Blockers: ___________

- [ ] ---
- [ ] _See `04_CLAUDE_INSTRUCTIONS/CONTEXT_LOADING_ORDER.md` for full v2.0 loading rules._


---

## Startup Reminder — GitHub Context Update Loop

After any meaningful state change this session, run the **GitHub Context Update Loop** (defined in `MASTER_INSTRUCTION_SET.md`).

Trigger it after:
- Completing a task or post loop
- - Changing active task status or next action
  - - Approving a workflow or major decision
    - - Ending a session with new progress
     
      - Update: `SHORT_TERM_CONTEXT.md`, `ACTIVE_TASKS.md`, and optionally `ASSET_INDEX.md` / `LONG_TERM_MEMORY.md`.
      - Then commit with: `Update context after [task name]`
     
      - Do not run after minor actions. Keep updates short and compressed.
