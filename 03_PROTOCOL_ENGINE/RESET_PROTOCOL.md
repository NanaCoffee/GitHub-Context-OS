# RESET PROTOCOL

## Version: 1.0
## Date: 2026-06-17

---

## Purpose
Defines the steps to perform a controlled context reset when Claude loses context, gets confused, or requires a clean restart.

---

## Trigger Conditions
Initiate a reset when:
- Claude produces repeated errors or hallucinations
- Context window appears full or corrupted
- Session goals have significantly shifted
- User explicitly requests a reset

---

## Reset Steps

### STEP 1: Capture State
- [ ] Save any in-progress work to WORKING_MEMORY.md
- [ ] Note the last completed action
- [ ] Flag any blocking issues

### STEP 2: Clear Working Memory
- [ ] Archive current WORKING_MEMORY.md content
- [ ] Clear WORKING_MEMORY.md to blank template

### STEP 3: Update Short-Term Context
- [ ] Update SHORT_TERM_CONTEXT.md with reset reason
- [ ] Record last known good state

### STEP 4: Re-initialise
- [ ] Run SESSION_INIT.md checklist from Step 1
- [ ] Confirm context loaded correctly
- [ ] Resume from last known good state

### STEP 5: Log Reset
- [ ] Add entry to 05_ARCHIVE/CHANGELOG.md
  - Date, Reason, Steps taken, Outcome

  ---

  ## Post-Reset Confirmation
  > "Reset complete. Context OS re-loaded. Resuming from: [LAST ACTION]. Ready."

  ---
  _A reset is not a failure — it is a controlled recovery._
