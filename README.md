# claude-todo

A Claude Code skill for managing todos.

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

**Option 1 — Ask Claude Code to install it:**

Open this repo in Claude Code and say:

> "Can you install the skill?"

Claude will copy it to `~/.claude/skills/todo/` for you.

**Option 2 — Manual:**

```bash
cp -r .claude/skills/todo ~/.claude/skills/todo
```

The `/todo` command will then be available in all your projects.
