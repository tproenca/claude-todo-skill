# AGENTS.md

Standing instructions and context for all agents working in this repository.

## Project

**devflow** is a collection of Claude Code skills for developer workflow utilities.
Skills live under `.claude/skills/` and are designed to be copied into `~/.claude/skills/` for personal use across projects, or packaged into a plugin for community distribution.

## Repository Structure

```
devflow/
├── .claude/
│   └── skills/
│       └── todo/
│           └── SKILL.md   # Todo manager skill
├── AGENTS.md
├── CLAUDE.md
└── README.md
```

## Conventions

- Each skill lives in its own subdirectory under `.claude/skills/<skill-name>/SKILL.md`.
- Skill instructions must be self-contained — no external dependencies or API calls unless clearly documented.
- Commands follow the pattern `/todo <action> <args>`.
- Keep skill files concise: behavior rules over prose.

## Adding a New Skill

1. Create `.claude/skills/<skill-name>/SKILL.md`.
2. Document commands, behavior rules, and edge cases.
3. Update `README.md` with the new skill.
4. Test locally by copying to `~/.claude/skills/<skill-name>/SKILL.md`.

## Publishing

Skills can be distributed two ways:
- **Manual**: users copy the `SKILL.md` file into `~/.claude/skills/<skill-name>/`.
- **Plugin**: package into a plugin with `.claude-plugin/plugin.json` and submit to a marketplace.
