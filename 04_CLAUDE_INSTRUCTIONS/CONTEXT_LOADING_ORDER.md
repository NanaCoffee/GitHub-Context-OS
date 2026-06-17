# CONTEXT LOADING ORDER

## Version: 1.0
## Date: 2026-06-17

---

## Purpose
Defines the exact sequence in which Claude must load context files at the start of each session.

---

## Mandatory Loading Sequence

```
STEP 1  →  00_CONTEXT_CORE/SESSION_INIT.md
           (Start here every session)

           STEP 2  →  00_CONTEXT_CORE/CONTEXT_OS_MANIFEST.md
                      (Understand the full system structure)

                      STEP 3  →  00_CONTEXT_CORE/MASTER_INSTRUCTION_SET.md
                                 (Load operating rules)

                                 STEP 4  →  04_CLAUDE_INSTRUCTIONS/BEHAVIOR_RULES.md
                                            (Load behaviour rules)

                                            STEP 5  →  01_MEMORY_LAYERS/LONG_TERM_MEMORY.md
                                                       (Load persistent knowledge)

                                                       STEP 6  →  01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md
                                                                  (Load recent session context)

                                                                  STEP 7  →  02_OPERATIONAL_FILES/ACTIVE_TASKS.md
                                                                             (Load current task state)

                                                                             STEP 8  →  02_OPERATIONAL_FILES/PROJECT_REGISTRY.md
                                                                                        (Confirm active project)
                                                                                        ```

                                                                                        ---

                                                                                        ## Optional Loading (load on demand)

                                                                                        | File | When to Load |
                                                                                        |------|--------------|
                                                                                        | WORKING_MEMORY.md | When resuming mid-task |
                                                                                        | ASSET_INDEX.md | When referencing assets |
                                                                                        | RESET_PROTOCOL.md | When a reset is needed |
                                                                                        | ESCALATION_PROTOCOL.md | When an issue cannot be resolved |
                                                                                        | HANDOFF_PROTOCOL.md | At end of session |
                                                                                        | CHANGELOG.md | When reviewing history |

                                                                                        ---

                                                                                        ## Loading Confirmation
                                                                                        After completing the mandatory sequence, Claude should state:
                                                                                        > "Context OS loaded. [N] files read. Active project: [PROJECT]. Ready."

                                                                                        ---
                                                                                        _Keep this file updated if the loading order changes._
