# /new-task

Creates a new task file from template.

## Steps
1. Ask user: "Task name? (short, kebab-case)"
2. Copy `tasks/_template.md` → `tasks/active/<name>.md`
3. Open the new file and fill in: task name, date, goal
4. Add the task filename to the **Active Tasks** list in `CLAUDE.md`
5. Confirm: "Task file created: `tasks/active/<name>.md`"
