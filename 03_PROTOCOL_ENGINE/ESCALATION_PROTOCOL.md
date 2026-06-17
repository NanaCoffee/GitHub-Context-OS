# ESCALATION PROTOCOL

## Version: 1.0
## Date: 2026-06-17

---

## Purpose
Defines how to handle situations that cannot be resolved within normal session operations.

---

## Escalation Levels

### LEVEL 1 — Minor Issue
_Claude is uncertain or needs clarification._
- Action: Ask user directly for clarification
- Log: Note in WORKING_MEMORY.md

### LEVEL 2 — Task Blocker
_A task cannot proceed due to missing info or a blocker._
- Action: Flag as `[!]` in ACTIVE_TASKS.md
- Log: Document blocker in SHORT_TERM_CONTEXT.md under "Open Threads"
- Notify: Inform user of the blocker and proposed resolution

### LEVEL 3 — Context Failure
_Claude context is compromised or contradictory._
- Action: Initiate RESET_PROTOCOL.md
- Log: Record in CHANGELOG.md
- Notify: Inform user that a reset was performed

### LEVEL 4 — System Issue
_The Context OS itself has a structural problem._
- Action: Stop all tasks
- Log: Document fully in CHANGELOG.md with all details
- Notify: Alert user immediately with full description
- Resolution: User must review and approve fix before resuming

---

## Escalation Template
```
ESCALATION NOTICE
Level: [1/2/3/4]
Date: YYYY-MM-DD
Issue: [description]
Affected files/tasks: [list]
Proposed resolution: [steps]
Status: [Pending/Resolved]
```

---
_Escalations should be rare. A well-maintained Context OS prevents most issues._
