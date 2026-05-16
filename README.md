<div align="center">

<img src="robot.svg" alt="Claude Code" width="110">

  # claude-todo

  A [Claude Code](https://claude.ai/code) skill for managing todos.

  > *Because not everything deserves a ticket*

  [![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)](LICENSE)

</div>

---

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

## Natural language

Once the skill is loaded, you don't need to use `/todo` explicitly. Claude understands intent — just talk to it:

- *"remind me to update the changelog"* → adds a todo
- *"what's left to do?"* → lists open todos
- *"mark the auth PR as done"* → checks it off
- *"clean up the list and sort by priority"* → reprioritizes

## Acknowledgements

Inspired by [Nilmax Moura](https://github.com/nilmax), the undisputed king of todos that never get done.

## License

MIT
