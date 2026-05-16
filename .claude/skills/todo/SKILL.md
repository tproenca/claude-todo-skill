# Todo Skill

Manage a `TODO.md` file in the current project.

## Commands

- `/todo add <item> [#tag]` — add a new todo, optionally with a tag
- `/todo check <number>` — mark a todo as done (`[x]`)
- `/todo remove <number>` — delete a todo
- `/todo prioritize` — reorder open todos by priority (ask the user if unclear)
- `/todo list [#tag]` — list all todos with numbers; filter by tag if provided
- `/todo tag <number> #tag` — attach a tag to an existing todo

## Behavior

- Always read `TODO.md` before making any change.
- Display todos as a numbered list so the user can reference items by number.
- Numbers are 1-based and reflect the current order in the file.
- Tags are inline at the end of the item text, formatted as `#tag`.
- An item can have multiple tags: `[ ] Review PRD #backend #docs`.
- Completed items (`[x]`) are kept at the bottom of the file, below open items.
- If `TODO.md` does not exist, create it when the first item is added. If the current directory is inside a git repository (check with `git rev-parse --is-inside-work-tree`), ask the user: "TODO.md will be created — add it to .gitignore so it stays local?" If they say yes, append `TODO.md` to the project's `.gitignore` (creating it if needed) before writing the file.
- After every write operation, confirm what changed in one short sentence.
- Never reformat or reorder items unless the user explicitly runs `prioritize`.
