# Impeccable frontend design skill

This repository tracks [Impeccable](https://github.com/pbakaus/impeccable) as a Git submodule pinned to a reviewed upstream commit. Impeccable provides one frontend design skill with 24 design commands and a deterministic UI anti-pattern detector. It supports Codex, Claude Code, Cursor, and other coding agents.

## Set up for Codex

Clone this repository with its submodule:

```bash
git clone --recurse-submodules https://github.com/mehjon/everything-claude-code.git
```

If you already cloned it without submodules:

```bash
git submodule update --init --recursive
```

From the repository root, link Impeccable's Codex skill and project hook:

```bash
npx impeccable link --source=.impeccable --providers=codex
```

Restart or reload Codex. The skill is available as `$impeccable`; its commands include `init`, `shape`, `critique`, `audit`, `polish`, `layout`, `typeset`, `adapt`, `harden`, and `optimize`. Review and approve the project hook in Codex when prompted.

## Update Impeccable

Update the pinned submodule to upstream `main`, then relink the Codex files:

```bash
git submodule update --remote .impeccable
npx impeccable link --source=.impeccable --providers=codex
```

Review the upstream release notes and changes before committing the updated submodule pointer or generated provider files.

Impeccable is distributed under the Apache License 2.0. Its source and license are retained in the `.impeccable` submodule.
