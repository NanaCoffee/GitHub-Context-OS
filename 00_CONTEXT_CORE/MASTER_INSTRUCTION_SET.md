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


---

### LinkedIn Post Execution Loop

#### Purpose

Use this loop whenever Nas / Geoffrey approves a LinkedIn post for publishing, review, follow-up, or performance tracking.

The goal is to avoid recreating the same instructions manually every time.

#### Trigger

Run this loop when the user asks for any of the following:
- publish a LinkedIn post
- - review a published LinkedIn post
  - - post a self-comment
    - - DM someone connected to a LinkedIn post
      - - record LinkedIn post performance
        - - continue a LinkedIn content workflow
         
          - #### 1. Draft / Approval Stage
         
          - - Only use post copy approved by Nas or ChatGPT.
            - - Do not make creative changes after approval unless explicitly requested.
              - - If a factual correction appears, update only the relevant wording and confirm before publishing.
                - - Keep Nas's LinkedIn content practical, observational, calm, and credible.
                  - - Do not make it salesy.
                    - - Do not create public Coffee Performance sales content.
                     
                      - #### 2. Publishing Stage
                     
                      - When publishing:
                      - - Open LinkedIn.
                        - - Publish the approved post exactly as provided.
                          - - Attach an image only if explicitly approved.
                            - - Tag a company or person only if explicitly approved and LinkedIn clearly identifies the correct account.
                              - - Do not add extra hashtags.
                                - - Do not add unapproved links.
                                  - - Do not send DMs during publishing unless instructed.
                                    - - Do not reply to comments.
                                      - - Do not accept or reject connection requests.
                                        - - Do not take unrelated LinkedIn actions.
                                         
                                          - #### 3. Post-Publish Report
                                         
                                          - After publishing, report:
                                         
                                          - ```
                                            Task:
                                            Status:
                                            Post published: Yes/No
                                            Post URL, if available:
                                            Exact posting time shown, or relative time if LinkedIn does not show exact time:
                                            Image attached: Yes/No
                                            Tags used:
                                            Copy changes made:
                                            Other actions taken:
                                            Issues:
                                            Stopped:
                                            GitHub Context Update Needed: Yes/No
                                            ```

                                            #### 4. Relationship Follow-Up Stage

                                            If the post is connected to a person, founder, company, sample, meeting, or collaboration:
                                            - Send a DM only after Nas explicitly approves.
                                            - - Message only the confirmed person.
                                              - - Do not message multiple people unless approved.
                                                - - Include the post link if relevant.
                                                  - - Keep the message polite, specific, and non-salesy.
                                                    - - Report: recipient, message sent status, post link included, other actions, issues, and stopped status, and GitHub Context Update Needed: Yes/No.
                                                     
                                                      - #### 5. Waiting Period
                                                     
                                                      - After publishing and any approved DM:
                                                      - - Do not self-comment immediately unless instructed.
                                                        - - Wait 24 hours before performance review.
                                                          - - Do not chase replies.
                                                            - - Do not take extra LinkedIn actions.
                                                             
                                                              - #### 6. 24-Hour Review Stage
                                                             
                                                              - At the review checkpoint, collect:
                                                              - - Impressions / views
                                                                - - Members reached
                                                                  - - Reactions
                                                                    - - Comments
                                                                      - - Reposts
                                                                        - - Saves
                                                                          - - Sends
                                                                            - - Profile viewers from this post
                                                                              - - Followers gained
                                                                                - - Connection requests, if visible
                                                                                  - - Notable comments
                                                                                    - - Comments needing reply
                                                                                      - - Audience demographics, if shown
                                                                                        - - Any DM reply connected to the post
                                                                                         
                                                                                          - Do not engage with the post during review unless instructed.
                                                                                         
                                                                                          - #### 7. Decision Stage
                                                                                         
                                                                                          - After review:
                                                                                          - - If reach is good but engagement is low, recommend a self-comment.
                                                                                            - - If there are comments, recommend natural replies instead of using a planned self-comment.
                                                                                              - - If the post performs poorly, record the lesson and adjust the next post.
                                                                                                - - Do not self-comment or reply without approval.
                                                                                                 
                                                                                                  - #### 8. Record Stage
                                                                                                 
                                                                                                  - After each completed LinkedIn post loop, run the GitHub Context Update Rule if the workflow caused a meaningful state change.
                                                                                                 
                                                                                                  - Update:
                                                                                                  - - `SHORT_TERM_CONTEXT.md` with post topic, date, post URL, status, key metrics, follow-up action, and next checkpoint.
                                                                                                    - - `ACTIVE_TASKS.md` if there is a new active checkpoint.
                                                                                                      - - `ASSET_INDEX.md` only if the post URL or related asset needs indexing.
                                                                                                        - - `LONG_TERM_MEMORY.md` only if a stable rule or major decision was created.
                                                                                                         
                                                                                                          - #### 9. Token Efficiency Rule
                                                                                                         
                                                                                                          - - Do not ask for repeated instructions that are already covered by this loop.
                                                                                                            - - Only ask for missing information required for the current stage.
                                                                                                             
                                                                                                              - #### 10. Boundary Rule
                                                                                                             
                                                                                                              - Do not publish Coffee Performance offers, booking links, payment links, launch announcements, or sales content.
                                                                                                             
                                                                                                              - Nas's LinkedIn content should remain focused on:
                                                                                                              - - personal credibility
                                                                                                                - - coffee
                                                                                                                  - - hospitality
                                                                                                                    - - service rhythm
                                                                                                                      - - training
                                                                                                                        - - product quality
                                                                                                                          - - café operations
                                                                                                                            - - real-world observations


---

### GitHub Context Update Rule

#### Purpose

Claude must treat GitHub Context OS as the compressed operating memory layer for the project.

After completing any meaningful workflow, Claude must check whether the GitHub Context Update Loop should run.

This reduces repeated prompting, prevents context loss, and improves token efficiency across future sessions.

#### When to Run

Run the GitHub Context Update Loop after meaningful state changes, including:
- A LinkedIn post is published
- - A LinkedIn post performance review is completed
  - - A post follow-up DM is sent
    - - A reusable workflow is added
      - - A Drive cleanup batch is completed
        - - A project task changes status
          - - A next action changes
            - - A major decision is approved
              - - A new important contact, relationship, or opportunity is created
                - - A file location or asset status changes
                  - - A session ends with useful progress that should be preserved
                   
                    - #### When Not to Run
                   
                    - Do not update GitHub after minor actions, including:
                    - - Tiny wording edits
                      - - Simple confirmations
                        - - One-off advice
                          - - Temporary drafts that were not approved
                            - - Actions that do not change project state
                              - - Duplicate notes already recorded elsewhere
                               
                                - #### Files to Consider
                               
                                - When the loop runs, update only the files that are relevant.
                               
                                - **`01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md`** — Use for:
                                - - What happened this session
                                  - - What was completed
                                    - - What is active now
                                      - - What the next checkpoint is
                                        - - What should not be repeated
                                         
                                          - **`02_OPERATIONAL_FILES/ACTIVE_TASKS.md`** — Use for:
                                          - - Current task status
                                            - - Completed task updates
                                              - - Next active task
                                                - - Checkpoint dates or review windows
                                                 
                                                  - **`02_OPERATIONAL_FILES/ASSET_INDEX.md`** — Use only when:
                                                  - - A new important asset was created
                                                    - - A post URL needs recording
                                                      - - A Drive file/location changed
                                                        - - An external reference needs indexing
                                                         
                                                          - **`01_MEMORY_LAYERS/LONG_TERM_MEMORY.md`** — Use only when:
                                                          - - A stable project rule is approved
                                                            - - A repeated workflow becomes permanent
                                                              - - A major strategic decision is made
                                                                - - A durable operating principle is created
                                                                 
                                                                  - #### Commit Rule
                                                                 
                                                                  - After updating GitHub files, Claude must commit the changes.
                                                                 
                                                                  - Commit message format: `Update context after [workflow/task name]`
                                                                 
                                                                  - Examples:
                                                                  - - `Update context after Oliiv LinkedIn post`
                                                                    - - `Update context after LinkedIn performance review`
                                                                      - - `Add LinkedIn Post Execution Loop`
                                                                        - - `Update active tasks after Drive cleanup`
                                                                          - - `Record GitHub Context Update Rule`
                                                                           
                                                                            - #### Reporting Format
                                                                           
                                                                            - After completing a GitHub Context update, report:
                                                                           
                                                                            - ```
                                                                              TASK:
                                                                              STATUS:
                                                                              FILES UPDATED:
                                                                              SUMMARY OF CHANGES:
                                                                              COMMIT MADE:
                                                                              COMMIT MESSAGE:
                                                                              COMMIT HASH:
                                                                              ISSUES:
                                                                              NEXT ACTION:
                                                                              ```

                                                                              #### Constraints

                                                                              - Do not rewrite the whole repository.
                                                                              - - Do not duplicate old context.
                                                                                - - Keep updates short and compressed.
                                                                                  - - Do not move or edit Google Drive source-of-truth files unless explicitly instructed.
                                                                                    - - GitHub is the context and memory layer, not the main storage layer.
                                                                                      - - Stop and report if unsure whether something belongs in short-term, active tasks, asset index, or long-term memory.
                                                                                       
                                                                                        - #### Default Behaviour
                                                                                       
                                                                                        - At the end of any meaningful completed task, Claude must include this check in its report:
                                                                                       
                                                                                        - > **GitHub Context Update Needed: Yes/No**
                                                                                          >
                                                                                          > If Yes, Claude should either:
                                                                                          > - Run the GitHub Context Update Loop immediately if already approved by standing instruction, or
                                                                                          > - - State exactly which files should be updated if execution permission is unclear.


---

### Token Efficiency Start Protocol

#### Purpose

Claude must begin every session by preserving tokens and avoiding unnecessary context loading.

The goal is to continue from the compressed project context instead of rebuilding the whole project history.

#### Trigger

Run this protocol at the start of every Claude session, before any execution work.

#### Startup Behaviour

At the start of each session, Claude must:
- Read `00_CONTEXT_CORE/SESSION_INIT.md`
- - Read `01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md`
  - - Read `02_OPERATIONAL_FILES/ACTIVE_TASKS.md`
    - - Read `02_OPERATIONAL_FILES/ASSET_INDEX.md` only if file locations, post URLs, Drive locations, or asset status are needed
      - - Read `01_MEMORY_LAYERS/LONG_TERM_MEMORY.md` only if project rules, boundaries, or stable memory are unclear
       
        - #### Token Efficiency Rules
       
        - Claude must:
        - - Avoid reading the whole repository unless explicitly instructed
          - - Avoid inspecting Google Drive unless the task requires it
            - - Avoid re-checking files already confirmed in the current session
              - - Avoid repeating long summaries unless requested
                - - Avoid rebuilding workflows already stored in MASTER_INSTRUCTION_SET.md
                  - - Use existing workflows before asking for new instructions
                    - - Ask only for missing information needed to complete the current task
                      - - Keep reports compact unless Nas asks for full detail
                        - - Preserve exact filenames, links, dates, and task statuses
                          - - Stop and ask if the task scope is unclear rather than exploring broadly
                           
                            - #### Workflow Detection
                           
                            - Before execution, Claude must check whether the task belongs to an existing workflow, including:
                            - - LinkedIn Post Execution Loop
                              - - GitHub Context Update Rule
                                - - Usage Limit / Session Close Protocol
                                  - - Drive cleanup / file control workflows, if present
                                    - - Any other stored workflow in MASTER_INSTRUCTION_SET.md
                                     
                                      - If a matching workflow exists, Claude must use it instead of recreating instructions manually.
                                     
                                      - #### Startup Report
                                     
                                      - After reading the minimum context, Claude should give a compact startup report:
                                     
                                      - ```
                                        SESSION STARTED:
                                        CONTEXT READ:
                                        ACTIVE TASK:
                                        KNOWN NEXT ACTION:
                                        WORKFLOW DETECTED:
                                        MISSING INFO:
                                        READY TO PROCEED:
                                        ```

                                        #### Constraints

                                        - Do not start broad audits by default.
                                        - - Do not inspect unrelated folders or files.
                                          - - Do not ask Nas to repeat context already stored in GitHub.
                                            - - Do not expand the task unless instructed.
                                              - - Token efficiency is more important than exhaustive context loading.

## Usage Limit / Session Close Protocol

### Purpose

Claude must protect project continuity when usage limits, context limits, or long-session fatigue appear.

The goal is to avoid losing progress, decisions, task status, next actions, file changes, commits, or pending checkpoints.

### Trigger

Run this protocol when:

- Nas mentions usage limit
- - Claude detects the session is becoming long
  - - Claude is close to context or usage limits
    - - a major workflow has just completed
      - - a task cannot safely continue without recording progress
        - - Nas says /pause, /next, usage limit, approaching limit, close session, save context, or similar
         
          - ### Required Action
         
          - When triggered, Claude must stop new execution and create a compact session close update.
         
          - Claude should record:
         
          - - what was completed
            - - what is currently active
              - - what is blocked
                - - next recommended action
                  - - files changed
                    - - commits made
                      - - pending checkpoints
                        - - anything Nas must not repeat next session
                         
                          - ### GitHub Update
                         
                          - If meaningful progress occurred, run the GitHub Context Update Rule.
                         
                          - Update only relevant files:
                         
                          - - 01_MEMORY_LAYERS/SHORT_TERM_CONTEXT.md for session progress and next checkpoint
                            - - 02_OPERATIONAL_FILES/ACTIVE_TASKS.md for current task status
                              - - 02_OPERATIONAL_FILES/ASSET_INDEX.md only if new URLs/assets/files matter
                                - - 01_MEMORY_LAYERS/LONG_TERM_MEMORY.md only if a stable rule or major decision was created
                                 
                                  - Commit changes with one of these messages:
                                 
                                  - - Update context before session close
                                    - - Update context before usage limit
                                      - - Update context after completed workflow
                                       
                                        - ### Reporting Format
                                       
                                        - After saving context, report:
                                       
                                        - ```
                                          TASK:
                                          STATUS:
                                          SESSION CLOSE SUMMARY:
                                          FILES UPDATED:
                                          COMMIT MADE:
                                          COMMIT MESSAGE:
                                          COMMIT HASH:
                                          NEXT ACTION:
                                          SAFE TO STOP: Yes/No
                                          GITHUB CONTEXT UPDATE NEEDED: Yes/No
                                          ```

                                          ### Constraints

                                          - Do not start new work after this protocol is triggered.
                                          - - Do not inspect unrelated files.
                                            - - Do not rewrite old context.
                                              - - Keep the update compressed.
                                                - - Prioritise continuity over completeness.
                                                  - - If no meaningful progress occurred, say GitHub update is not needed and explain briefly.
                                                    - - If uncertain what to save, save only the confirmed completed work, active task, and next action.


---

## Product Value Lens — Revenue Idea Filter

Every new revenue idea, offer, product concept, service concept, or workflow expansion must be checked against the Product Value Lens before it is developed.

A strong idea should clearly answer at least two of the three lenses. A priority idea should answer all three.

### 1. Solution

Does the idea make a painful problem go away?

Examples:

- removes confusion
- - reduces waste
  - - fixes repeated manual work
    - - clarifies a broken workflow
      - - helps the buyer make a decision
        - - removes a recurring operational headache
         
          - ### 2. Convenience
         
          - Does the idea make the buyer's life faster, simpler, easier, or less stressful?
         
          - Examples:
         
          - - one focused session instead of a long programme
            - - clear written output
              - - simple next actions
                - - less admin
                  - - fewer tools
                    - - reduced decision fatigue
                      - - no unnecessary setup
                       
                        - ### 3. Experience
                       
                        - Does the buyer pay for a valuable feeling?
                       
                        - Examples:
                       
                        - - clarity
                          - - control
                            - - relief
                              - - confidence
                                - - professionalism
                                  - - calm
                                    - - status
                                      - - feeling less behind
                                        - - feeling their business is easier to run
                                         
                                          - ### Commercial Priority Filter
                                         
                                          - After the three lenses, check whether the idea is:
                                         
                                          - - private-testable
                                            - - fast to prove
                                              - - connected to revenue
                                                - - low manual workload
                                                  - - deliverable with current tools
                                                    - - useful for proof capture
                                                      - - not dependent on public launch
                                                        - - not dependent on a website, payment link, automation, or large infrastructure build
                                                         
                                                          - ### Operating Rule
                                                         
                                                          - Do not build from excitement alone.
                                                          - Do not create products from brainstorming.
                                                          - Do not expand an idea unless it has passed the Product Value Lens and Commercial Priority Filter.
                                                         
                                                          - Coffee is now treated as a parked specialist vertical, not the default commercial route.
                                                         
                                                          - The current broader direction is:
                                                          - AI-assisted operations clarity for small service businesses.
                                                         
                                                          - The first non-coffee private revenue experiment is:
                                                          - One-session AI tool clarity review / AI Tool Role Audit at £350.
