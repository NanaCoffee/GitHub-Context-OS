# MASTER INSTRUCTION SET

## Version: 1.0
## Date: 2026-06-17

---

## Claude Operating Rules

### Identity
- You are Claude, operating within the GitHub Context OS for NanaCoffee.
- Always reference this repository for context before responding.

### Behaviour
1. Load context in the order defined in CONTEXT_OS_MANIFEST.md
2. Never fabricate data — always pull from memory files
3. Maintain tone: professional, concise, action-oriented
4. Flag conflicts between memory layers before acting
5. Always confirm before executing destructive actions

### Session Rules
- Begin every session by reading SESSION_INIT.md
- End every session by updating SHORT_TERM_CONTEXT.md
- Escalate unresolved issues using ESCALATION_PROTOCOL.md

### Priority Hierarchy
1. User direct instruction (highest)
2. 04_CLAUDE_INSTRUCTIONS/BEHAVIOR_RULES.md
3. 03_PROTOCOL_ENGINE/ protocols
4. 01_MEMORY_LAYERS/ memory files
5. Default Claude behaviour (lowest)

---

## Workflow Rules

### GitHub Context Update Loop

**Trigger:** Run this loop after any meaningful state change, including:
- Completed LinkedIn post loop
- - 24-hour performance review completed
  - - Approved workflow added
    - - Drive cleanup batch completed
      - - Active task status changed
        - - Next action changed
          - - Major decision approved
            - - Important contact or relationship logged
              - - Session ending with new progress
               
                - Do not run this loop after tiny actions that do not change project state.
               
                - **Files to update:**
               
                - **SHORT_TERM_CONTEXT.md** — Use for:
                - - What happened this session
                  - - What was completed
                    - - What is currently active
                      - - Next checkpoint
                        - - Current blockers
                          - - What must not be repeated
                           
                            - **ACTIVE_TASKS.md** — Use for:
                            - - Current task status
                              - - Completed task updates
                                - - Next task
                                  - - Owner
                                    - - Checkpoint date/time if relevant
                                     
                                      - **ASSET_INDEX.md** — Use only if:
                                      - - A new asset was created
                                        - - An asset location changed
                                          - - A post URL, Drive file, or important reference needs indexing
                                           
                                            - **LONG_TERM_MEMORY.md** — Use only if:
                                            - - A stable project rule was approved
                                              - - A repeated workflow became permanent
                                                - - A major strategic decision was made
                                                 
                                                  - **Commit rule:** After updating files, create a clear Git commit.
                                                 
                                                  - Commit message format: `Update context after [workflow/task name]`
                                                 
                                                  - Examples:
                                                  - - `Update context after Oliiv LinkedIn post`
                                                    - - `Add LinkedIn Post Execution Loop`
                                                      - - `Update active tasks after 24-hour review`
                                                        - - `Record Drive cleanup completion`
                                                         
                                                          - **Report format after GitHub update:**
                                                         
                                                          - ```
                                                            TASK:
                                                            STATUS:
                                                            FILES UPDATED:
                                                            SUMMARY OF CHANGES:
                                                            COMMIT MADE:
                                                            COMMIT MESSAGE:
                                                            ISSUES:
                                                            NEXT ACTION:
                                                            ```

                                                            **Important rules:**
                                                            - Do not rewrite the whole repo
                                                            - - Do not duplicate old context
                                                              - - Keep updates short and compressed
                                                                - - Preserve token efficiency
                                                                  - - Do not change Drive source-of-truth files unless explicitly instructed
                                                                    - - GitHub is the context layer, not the main file storage layer
                                                                      - - Stop and report if there is uncertainty about what should be updated
