# skills

Agent skills for AI coding assistants, installable with [skills.sh](https://skills.sh/) and the Skills CLI.

[![skills.sh](https://skills.sh/b/tomshlomo/skills)](https://skills.sh/tomshlomo/skills)

Skills follow the [Agent Skills](https://agentskills.io/) format (`SKILL.md` with YAML frontmatter).

## Install

Install one skill globally (recommended for personal workflows):

```bash
npx skills add tomshlomo/skills@iron -g -y
```

Install into a project only:

```bash
npx skills add tomshlomo/skills@iron -y
```

List skills in this repo without installing:

```bash
npx skills add tomshlomo/skills -l
```

## Available skills

### iron

Clarifies requirements before implementation by asking focused text-based questions, one at a time, with numbered options in chat (not the built-in questions UI). Invoke with `/iron` when you want to remove ambiguity before coding.

**Use when:**

- Starting a feature or change where scope or trade-offs are unclear
- You want a short Q&A pass instead of jumping straight into code
- You prefer replying with option numbers rather than long free-text answers

## Adding skills

Add a new directory under `skills/<name>/` with a `SKILL.md` file. Optionally register it in `skills.sh.json` for grouping on [skills.sh](https://skills.sh/).

```bash
npx skills init my-new-skill
# move or merge into skills/my-new-skill/
```

## License

MIT
