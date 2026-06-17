# HANDOFF PROTOCOL

## Version: 1.0
## Date: 2026-06-17

---

## Purpose
Defines how to hand off context between sessions, tools, or collaborators so that continuity is preserved.

---

## End-of-Session Handoff

Run before closing any Claude session:

### Step 1: Complete Working Memory
- [ ] Ensure WORKING_MEMORY.md is up to date
- [ ] Move any keeper notes to SHORT_TERM_CONTEXT.md

### Step 2: Update Active Tasks
- [ ] Update task statuses in ACTIVE_TASKS.md
- [ ] Mark completed tasks as `[x]`
- [ ] Add any new tasks discovered during session

### Step 3: Write Session Summary
Update SHORT_TERM_CONTEXT.md with:
- What was accomplished
- What is pending
- Next session's first action

### Step 4: Commit to GitHub
- [ ] Commit all changed files to main branch
- [ ] Write clear commit message

---

## Cross-Tool Handoff
When handing context to another AI tool or system:
1. Export CONTEXT_OS_MANIFEST.md as system context
2. Include SHORT_TERM_CONTEXT.md as session briefing
3. Include ACTIVE_TASKS.md as task state

---

## Handoff Summary Template
```
HANDOFF SUMMARY
Date: YYYY-MM-DD
From: [Session/Tool]
To: [Next Session/Tool]
Status: [Ready/Needs Attention]
Last Action: 
Next Action: 
Notes: 
```

---
_A clean handoff ensures every session starts strong._
