---
Status: DRAFT
Owner: Nas
Created: 2026-07-02
Review Required: Yes
---

# KNOWLEDGE SAFETY PROTOCOL

## Purpose
Define where knowledge is stored and what is safe for NotebookLM, GitHub Context OS, and Drive.

Protect client privacy, business strategy, and work-in-progress materials.

## Storage Rules by Knowledge Type

| Type | Storage | GitHub | NotebookLM |
|------|---------|--------|-----------|
| Client-sensitive (names, feedback, meetings) | Drive only | NO | NO |
| Work-in-progress (drafts, rough ideas) | Drive or chat | NO | NO |
| Internal strategy (pricing, offer design) | Drive or GitHub context | Private only | NO |
| Approved, final, tested knowledge | GitHub or Drive | YES | YES |

## Client-Sensitive Material Definition

NEVER store in GitHub or NotebookLM:
- Client names, companies, contact details
- - Meeting outcomes, feedback, proprietary processes
  - - Pricing, contracts, deal terms
    - - Performance metrics (unless anonymized)
      - - Leak Review work = client-sensitive, stays in Drive
       
        - Store in Drive only. Reference in GitHub generically (e.g., "Private client meeting" not "Meeting with [Client]").
       
        - ## Task Logging Rule
       
        - ACTIVE_TASKS.md descriptions must not include client names.
        - Use anonymous placeholders: "Private client meeting" instead of "Meeting with [Client Name]".
       
        - ## NotebookLM Preparation Checklist
       
        - Before uploading anything to NotebookLM:
       
- [ ] Approved by Nas (final, not draft)
          - [ ] - [ ] Clean version (no corrections pending)
          - [ ] - [ ] No client-sensitive data (anonymized or excluded)
          - [ ] - [ ] Something Nas wants preserved long-term (not ephemeral)
         
          - [ ] If ANY check fails: DO NOT UPLOAD. Ask Nas first.
         
          - [ ] ## NotebookLM Forbidden Content
         
          - [ ] ✗ Draft posts (use published only with live links)
          - [ ] ✗ Client names, meeting outcomes, feedback
          - [ ] ✗ Pricing details, unapproved product ideas
          - [ ] ✗ Decision-making process or internal rationale
          - [ ] ✗ Unapproved ChatGPT exports or brainstorms
          - [ ] ✗ Unpublished research
         
          - [ ] ## NotebookLM Allowed Content
         
          - [ ] ✓ Published LinkedIn posts (with live links)
          - [ ] ✓ Confirmed operational procedures (tested, step-by-step)
          - [ ] ✓ Approved product descriptions (final versions)
          - [ ] ✓ Published case studies (anonymized)
          - [ ] ✓ Coffee operations knowledge (if approved for sharing)
          - [ ] ✓ General AI/business insights (published, sourced)
         
          - [ ] ## What Claude NEVER Does
         
          - [ ] ✗ Upload anything to NotebookLM without checklist review
          - [ ] ✗ Store client names in GitHub
          - [ ] ✗ Include internal strategy or pricing in NotebookLM
          - [ ] ✗ Share draft or unapproved content to NotebookLM
          - [ ] ✗ Assume "client work" can go to shared knowledge bases
          - [ ] ✗ Upload without explicit Nas approval
         
          - [ ] ## Pre-Upload / Pre-Log Checklist
         
          - [ ] - [ ] Knowledge type identified (client-sensitive, WIP, strategy, or approved/final)
          - [ ] - [ ] Storage location correct (Drive, GitHub context, or NotebookLM)
          - [ ] - [ ] No client names, pricing, or internal debate
          - [ ] - [ ] Nas approves storage location
          - [ ] - [ ] NotebookLM: all 4 checklist items passed
         
          - [ ] If ANY checkbox fails: STOP and ask Nas.
         
          - [ ] ## Stop & Wait Rules
         
          - [ ] STOP if: uncertain about knowledge type, storage location, client sensitivity, NotebookLM suitability, or Nas hasn't approved.
         
          - [ ] Ask first. Better to delay than expose sensitive material.
