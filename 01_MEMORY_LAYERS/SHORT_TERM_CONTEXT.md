---
Title: "SHORT TERM CONTEXT"
Version: 1.6
Last Updated: 2026-07-04
---

## Current Session Context

This file is updated at the END of every Claude session to preserve continuity.

---

## Last Session Summary

- **Date:** 2026-07-04
- **Project:** Coffee Performance Pilot — Fields Acton
- **What was accomplished:**
  - Active task corrected: Fields Acton — post-report follow-up / pilot conversion decision
  - Previous wording (Leak Review delivery loop) was outdated — face-to-face already done, report already sent
  - ACTIVE_TASKS.md updated to reflect actual current stage
  - SHORT_TERM_CONTEXT.md rewritten
  - No outreach started, no execution started, no client-facing messages created

## Claude Operating Behaviour (Current)

Claude should now:
- Start sessions by reading minimum required context (SESSION_INIT, SHORT_TERM_CONTEXT, ACTIVE_TASKS)
- Detect stored workflows before asking for repeated instructions
- Run LinkedIn workflows using the stored LinkedIn Post Execution Loop
- Check GitHub Context Update Needed: Yes/No after meaningful tasks
- Save context before usage/context limits or session close when meaningful progress occurred

## Live Operational Checkpoint

- **Active task:** Fields Acton — post-report follow-up / pilot conversion decision [~]
- **Face-to-face:** Done
- **Report sent to Sam:** 2026-07-01
- **Stage:** Awaiting response / conversion decision
- **No implementation started**
- **No assumption that Fields Acton has agreed to proceed**
- **Boundary:** No outreach unless Nas approves. No client-facing messages, pricing, or new product lane.
- **Oliiv LinkedIn review:** STALE [!] — awaiting controller confirmation

## Open Threads

- Fields Acton — awaiting Sam's response to the 2026-07-01 report
- Oliiv LinkedIn post 24-hour review — STALE, awaiting controller confirmation
- Status of Chris Averill reply — not checked

## Recent Decisions

| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-06-17 | Created GitHub-Context-OS repo | Needed structured Claude context system |
| 2026-06-17 | Adopted Context Loading Order V2 | Token efficiency — load minimum context only |
| 2026-06-17 | Created COMMANDS.md | Operating command reference for Nas, ChatGPT, and Claude |
| 2026-06-17 | Registered Nas LinkedIn Optimisation | Active workstream needs Context OS visibility |
| 2026-06-27 | Added LinkedIn Post Execution Loop | Automate repeated LinkedIn workflow steps |
| 2026-06-27 | Added GitHub Context Update Rule | Preserve session state and prevent context loss |
| 2026-06-27 | Added Token Efficiency Start Protocol | Load minimum context at session start |
| 2026-06-27 | Added Usage Limit / Session Close Protocol | Protect progress before context/usage limits |
| 2026-07-04 | Marked Oliiv review task [!] STALE | Task overdue, no controller confirmation, not executed |
| 2026-07-04 | Declared Fields Acton as Priority 1 active task | First CP pilot candidate confirmed by Nas |
| 2026-07-04 | Corrected task wording to post-report follow-up | Face-to-face done, report sent 2026-07-01, delivery loop framing was outdated |

---

This file should be rewritten each session, not appended.
