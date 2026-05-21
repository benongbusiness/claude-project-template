# CLAUDE.md

Project context hub. Keep this file lean. Load other docs only when needed.

---

## Project
- **Type:** Solo script / automation
- **Language:** _fill in_
- **Purpose:** _fill in_

## Repo Layout
```
src/          # main scripts
scripts/      # run/deploy helpers
tests/        # test files
tools/        # dev utilities
output/       # gitignored artifacts
tasks/        # per-task context files
docs/         # reference docs (load on demand)
.claude/      # Claude config and slash commands
```

---

## Context Loading Rules

Load these files **only when relevant** — do not load all upfront.

| Situation | Open this file |
|---|---|
| Touching structure, adding modules | `docs/architecture.md` |
| Making a tech/library choice | `docs/decisions.md` |
| Writing or running tests | `docs/testing.md` |
| Starting a new task | copy `tasks/_template.md` → `tasks/active/TASKNAME.md` |
| Task complete | move file → `tasks/done/` |
| Scratch notes / temp context | `docs/notes.md` |

---

## Conventions
- Scripts are standalone and runnable from repo root
- No hardcoded secrets — use `.env` (gitignored)
- Output goes in `output/` — never commit artifacts
- One task file per active workstream

## Active Tasks
_List active task files here so Claude knows what's in flight:_
- (none)

---

## Key Commands
```bash
# Run a script
python src/myscript.py

# Run tests
pytest tests/

# Check env
cat .env.example
```
