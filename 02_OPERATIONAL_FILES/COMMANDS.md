---
COMMANDS
Version: 1.0
Date: 2026-06-17
Workstream: GitHub Context OS / Token Efficiency

---

# GitHub Context OS — Operating Commands

## Purpose

This file defines the short operating commands used by Nas, ChatGPT, and Claude to reduce token waste and keep work operational.

**Default rule:**
Operate from the active task, not the full history.

---

## Commands

### /next

**Meaning:**
Return the single next logical operational action.

**Use when:**
Nas wants the next step without a full explanation.

**Output:**
- One action
- Brief reason only if needed
- No broad strategy unless requested

---

### /status

**Meaning:**
Return compact current status.

**Use when:**
Nas wants to know where the workstream stands.

**Output:**
- Active workstream
- Current status
- Next action
- Blockers if any

---

### /review

**Meaning:**
Review the current output, report whether it passes, and recommend the next action.

**Use when:**
Nas pastes a Claude output, file change report, draft, audit, or test result.

**Output:**
- Pass / fail / approve / revise
- Issues found
- Recommendation
- Next action

---

### /instruct claude

**Meaning:**
Create one tight, copy-paste-ready Claude instruction.

**Use when:**
The next step requires Claude execution.

**Output:**
- Workstream
- Task
- Context
- Output required
- Rules
- Stop condition

---

### /compress

**Meaning:**
Create an Active Context Card for the current workstream.

**Use when:**
A chat is getting long or token usage is high.

**Output:**
- Current status
- Approved decisions
- Boundaries
- Active task
- Do not do
- Next action

---

### /closeout

**Meaning:**
Create a compact handoff for a new session.

**Use when:**
A session is ending or approaching token limits.

**Output:**
- Workstream status
- Completed actions
- Active decisions
- Next action
- Files changed
- Risks / blockers

---

### /pause

**Meaning:**
Stop all work.

**Use when:**
Nas wants no further action.

**Output:**
- Paused confirmation only
- No new suggestions unless asked

---

### /map

**Meaning:**
Update or summarise the current operating map.

**Use when:**
Nas wants the project structure clarified.

**Output:**
- Active workstreams
- Source of truth
- Current next action
- Boundaries

---

## Behaviour Rules

- Commands should stay compact.
- Do not load full history unless explicitly needed.
- Do not create files unless the command asks for it.
- Do not perform destructive actions.
- Do not make legal, financial, public, or identity-changing changes without Nas approval.
- When unsure, ask for clarification before acting.

---

## Command Boundary

These commands are operating shortcuts, not shell commands.
They guide Claude behaviour inside project work.
They do not replace Git commands, system commands, or automation scripts.
