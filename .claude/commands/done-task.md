# /done-task

Archives a completed task.

## Steps
1. Ask user: "Which task file? (from `tasks/active/`)"
2. Update task file: set **Status** to `done`, add completion date
3. Move file: `tasks/active/<name>.md` → `tasks/done/<name>.md`
4. Remove from **Active Tasks** list in `CLAUDE.md`
5. Confirm: "Task archived: `tasks/done/<name>.md`"
