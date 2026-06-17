# GitHub Context OS

> A structured Context Operating System for managing Claude AI context layers, memory, and operational files across projects.
>
> **Owner:** NanaCoffee | **Version:** 1.0 | **Created:** 2026-06-17
>
> ---
>
> ## What is GitHub Context OS?
>
> GitHub Context OS is a structured repository system that gives Claude AI persistent memory and operational consistency across sessions. Instead of starting from scratch each time, Claude loads a defined set of context files in a specific order, enabling reliable, continuous, and controlled AI operations.
>
> ---
>
> ## Repository Structure
>
> ```
> GitHub-Context-OS/
> ├── 00_CONTEXT_CORE/              # Foundation files
> │   ├── CONTEXT_OS_MANIFEST.md    # System map & directory guide
> │   ├── MASTER_INSTRUCTION_SET.md # Claude operating rules
> │   └── SESSION_INIT.md           # Session startup checklist
> ├── 01_MEMORY_LAYERS/            # Claude memory system
> │   ├── LONG_TERM_MEMORY.md       # Persistent knowledge (rarely changes)
> │   ├── SHORT_TERM_CONTEXT.md     # Last session context (rewritten each session)
> │   └── WORKING_MEMORY.md         # In-session scratchpad (cleared each session)
> ├── 02_OPERATIONAL_FILES/        # Project & task management
> │   ├── ACTIVE_TASKS.md           # Current task board
> │   ├── PROJECT_REGISTRY.md       # All active projects
> │   └── ASSET_INDEX.md            # Master asset registry
> ├── 03_PROTOCOL_ENGINE/          # Rules for edge cases
> │   ├── RESET_PROTOCOL.md         # How to reset context
> │   ├── ESCALATION_PROTOCOL.md    # How to handle blockers
> │   └── HANDOFF_PROTOCOL.md       # End-of-session handoff
> ├── 04_CLAUDE_INSTRUCTIONS/      # Claude configuration
> │   ├── SYSTEM_PROMPT.md          # Ready-to-use system prompt
> │   ├── BEHAVIOR_RULES.md         # Detailed behaviour rules
> │   └── CONTEXT_LOADING_ORDER.md  # Exact file loading sequence
> └── 05_ARCHIVE/                  # History & logs
>     └── CHANGELOG.md              # All changes logged here
> ```
>
> ---
>
> ## How to Use
>
> ### Quick Start
> 1. Copy the system prompt from `04_CLAUDE_INSTRUCTIONS/SYSTEM_PROMPT.md`
> 2. 2. Paste it into Claude's system prompt field
>    3. 3. At session start, load files in the order defined in `CONTEXT_LOADING_ORDER.md`
>       4. 4. Begin working — Claude will operate with full context
>         
>          5. ### Session Flow
>          6. ```
>             START → SESSION_INIT.md → Load context files → Work → Update tasks & memory → Commit → END
>             ```
>
> ---
>
> ## Context Loading Order
>
> | Step | File | Purpose |
> |------|------|---------|
> | 1 | SESSION_INIT.md | Start checklist |
> | 2 | CONTEXT_OS_MANIFEST.md | System map |
> | 3 | MASTER_INSTRUCTION_SET.md | Operating rules |
> | 4 | BEHAVIOR_RULES.md | Behaviour rules |
> | 5 | LONG_TERM_MEMORY.md | Persistent knowledge |
> | 6 | SHORT_TERM_CONTEXT.md | Recent context |
> | 7 | ACTIVE_TASKS.md | Task state |
> | 8 | PROJECT_REGISTRY.md | Active projects |
>
> ---
>
> ## Protocols
>
> | Situation | Protocol |
> |-----------|----------|
> | Claude is confused or context is broken | RESET_PROTOCOL.md |
> | Task is blocked or unresolvable | ESCALATION_PROTOCOL.md |
> | Ending a session | HANDOFF_PROTOCOL.md |
>
> ---
>
> *Built by NanaCoffee — 2026*
