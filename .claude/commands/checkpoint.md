# /checkpoint

Saves current session progress to the active task file. Use before context gets long.

## Steps
1. Identify the current active task file from `CLAUDE.md`
2. Append to that task file under a `## Checkpoint — YYYY-MM-DD HH:MM` section:
   - What was done this session
   - Current state of each step (check off completed)
   - Any new decisions made
   - Where to resume next session
3. Confirm: "Checkpoint saved to `tasks/active/<name>.md`"
