---
Status: DRAFT
Owner: Nas
Created: 2026-07-02
Review Required: Yes
---

# DECISION AND HANDOFF PROTOCOL

## Purpose
Define how decisions from Nas/ChatGPT flow to Claude action and logging.

## Decision Triggers
Log when approved: revenue ideas, workflows, strategy shifts, major decisions.
Do NOT log: brainstorms, unapprov ideas, one-off advice.

## Required Fields
- Decision name
- Approval date & approver
- Rationale (why approved)
- Boundaries (constraints)
- Status (active/paused)

Store in LONG_TERM_MEMORY.md "Recent Decisions" table.

## Three Approval Types

**Type A: "Do This"**
- Language: "Publish", "Build", "Implement", "Update"
- Claude action: Execute, log in GitHub, commit
- Example: "Publish post" → publish + log + commit

**Type B: "Explore With Nas"**
- Language: "Good idea, check with Nas", "Worth exploring", "Need Nas's input"
- Claude action: Report to chat only, do NOT update GitHub
- Example: "Check with Nas first" → report to chat, wait for Nas approval

**Type C: "Remember This"**
- Language: "Log this", "Remember for next time", "Document this"
- Claude action: Ask Nas "Should I log this?" before recording

## Approval Logging
- Who: Claude Execution (after approval)
- What: ChatGPT approvals above threshold
- Where: LONG_TERM_MEMORY.md Recent Decisions table
- Commit: "Log decision: [name] approved by [approver]"

## Claude Escalation Rules (STOP & ASK)
- Approval language ambiguous → ask for clarification
- Conflicts with existing rule → report, ask precedence
- Outside Claude authority → escalate
- Blocked waiting for approval → document, report
- Type C without explicit Nas approval → ask first

## What Claude NEVER Does
- Execute Type A without explicit "do this"
- Log decision without approval
- Assume "sounds good" = approval
- Proceed on Type B without asking Nas
- Override decisions without new approval
- Create products without Type A approval

## Pre-Action Checklist
- [ ] Approval language is clear (not "maybe")
- [ ] Approver is Nas or ChatGPT
- [ ] Boundaries are understood
- [ ] No conflict with existing decisions
- [ ] Ready to log and commit

If ANY checkbox fails: STOP and ask Nas.

## Stop & Wait Rules
STOP if: ambiguous language, conflict, outside authority, blocked, Nas says "wait", or commit fails.
