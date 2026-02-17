# Contributing to Intent Migration Toolkit

This repo contains tools for migrating Discord communities to Intent. Nothing is implemented yet — just scaffolding.

## Pick an Issue

Check the [issues](https://github.com/IntentAi/intent-migrate/issues). Look at **blocking relationships** on the right side — some work depends on other issues landing first. Comment to claim, wait for assignment.

## Branching

Work is organized into phases. Check which phase branch is active or ask a maintainer.

```
git checkout <phase-branch> && git pull origin <phase-branch>
git checkout -b <phase-branch>/1-exporter-bot
```

No active phase branch? Use `feat/<issue>-description` off `dev`. PR against the **phase branch**, not dev or main.

## Commits

Conventional commits, reference the issue, one logical change each.

```
feat(exporter): extract channel list from Discord API [refs #1]

Uses discord.js to pull server structure including categories,
text/voice channels, topics, and position ordering.
```

## Tech Stack

- TypeScript for Discord-side tools (discord.js)
- TypeScript or Python for Intent-side tools (intent.js / intent.py)

## License

MIT
