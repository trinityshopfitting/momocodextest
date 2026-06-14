# Codex Conversation - 2026-06-14

## Topic

How to upload Codex conversation context, rules, and notes to GitHub so they can be pulled from other devices.

## Decisions

- Use GitHub repositories for durable files, not raw Codex local state.
- Store shared Codex rules in `AGENTS.md`.
- Store project-level Codex configuration in `.codex/config.toml` when needed.
- Store conversation summaries in `docs/codex-history/`.
- Do not commit `~/.codex/auth.json`, raw threads, sessions, memories, logs, or other private local state.

## Current GitHub Context

- Connected GitHub account: `trinityshopfitting`.
- New repository created on GitHub: `trinityshopfitting/momocodextest`.

## Useful Commands

```bash
git status
git add README.md AGENTS.md .gitignore docs/codex-history
git commit -m "Add Codex notes and rules"
git push -u origin main
```

