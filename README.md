# Skills Repository

This repository contains reusable AI interaction skills.

## Structure

- `skills/<skill-name>/SKILL.md` — Skill definitions

## Included Skills

### ContextFit

A structured workflow for achieving high-quality AI outputs with minimal context:
1. Clarify the desired outcome
2. Make key decisions via multiple-choice questions
3. Choose between solution options
4. Receive fully worked, standalone results

```bash
npx skills add https://github.com/klosebrothers/skills --skill contextfit
```

## Usage

### npx skills

```bash
`npx skills add https://github.com/klosebrothers/skills --skill <skill-name>`
```

## Conventions

- One folder per skill under `skills/`
- Each skill is defined in a `SKILL.md` file
- Skills start with YAML frontmatter (`name`, `description`, `version`, `author`)
