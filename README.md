# devflow

Claude Code skills for developer workflow utilities.

## Skills

### `/todo`

Manage a `TODO.md` file in any project.

| Command | Description |
|---|---|
| `/todo add <item> [#tag]` | Add a new todo |
| `/todo list [#tag]` | List todos with numbers; filter by tag |
| `/todo check <number>` | Mark a todo as done |
| `/todo remove <number>` | Delete a todo |
| `/todo prioritize` | Reorder open todos by priority |
| `/todo tag <number> #tag` | Tag an existing todo |

## Installation

Copy the skill into your personal Claude Code skills folder:

```bash
cp -r .claude/skills/todo ~/.claude/skills/todo
```

The `/todo` command will then be available in all your projects.
