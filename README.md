# skills

[![skills.sh](https://skills.sh/b/jonathanfilbert/skills)](https://skills.sh/jonathanfilbert/skills)

Personal [agent skills](https://skills.sh) by Jonathan Filbert.

## Install

Any agent, via [skills.sh](https://skills.sh):

```bash
npx skills add jonathanfilbert/skills
```

Claude Code, as a plugin marketplace:

```
/plugin marketplace add jonathanfilbert/skills
/plugin install kartu-kredit-id@jonathanfilbert-skills
```

## Skills

| Skill | What it does |
| --- | --- |
| [`kartu-kredit-id`](skills/kartu-kredit-id/SKILL.md) | Indonesia-only credit card research: miles, points, cashback, devaluation checks, large one-off spends (e.g. wedding). Search-first, issuer sources over aggregators. |

## Adding a skill

Create `skills/<name>/SKILL.md` with `name` (lowercase, hyphens) and `description` frontmatter. Scaffold with `npx skills init <name>`.

Then add a plugin entry for it to [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json) (`"source": "./"`, `"skills": ["./skills/<name>"]`) and run `claude plugin validate ./`.
