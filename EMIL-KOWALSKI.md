# Emil Kowalski design-engineering skills

This repository tracks Emil Kowalski’s official [skills collection](https://github.com/emilkowalski/skills) as a Git submodule, pinned to an upstream commit. The collection is licensed under MIT.

The main website-focused skill is `emil-design-eng`. Emil describes it as mostly animation, with additional design advice. For broader website design work, the collection also includes `apple-design` for interface principles, `prototype` for comparing UI directions, `pick-ui-library` for choosing dependable UI components, `break-ui` for stress-testing edge cases, and `mobile-native` for touch and small-screen behavior.

## Install for Codex

From this repository root, install the main skill for all Codex projects:

```bash
npx skills@latest add ./.emil-skills --skill emil-design-eng --agent codex --global
```

To add the complementary website skills as well:

```bash
npx skills@latest add ./.emil-skills --skill apple-design prototype pick-ui-library break-ui mobile-native --agent codex --global
```

Restart or reload Codex after installation. The skills will be available across projects in the Codex environment.

## Update the pinned source

```bash
git submodule update --remote .emil-skills
```

Review the upstream changes, then install the selected skills again from this checkout.
