# Issue tracker: Beads (bd)

Issues and specs for this repo live in **beads (bd)**, a dolt-backed issue tracker. Use the `bd` CLI for all operations.

## Conventions

- **Find available work**: `bd ready`
- **View an issue**: `bd show <id>`
- **Claim work**: `bd update <id> --claim`
- **Complete work**: `bd close <id>`
- **Push data to remote**: `bd dolt push`
- **Full workflow context**: `bd prime`
- **Persistent knowledge**: `bd remember <note>` — use instead of MEMORY.md files

Triage state is recorded as labels on each issue (see `triage-labels.md` for the role strings).

## When a skill says "publish to the issue tracker"

Create an issue with `bd`. The exact command depends on the context — run `bd prime` for the available subcommands.

## When a skill says "fetch the relevant ticket"

Run `bd show <id>`.

## When a skill says "apply a triage label"

Run `bd update <id> --label <label-string>`. The label strings are defined in `triage-labels.md`.

## Wayfinding operations

Used by `/wayfinder`. The **map** is a single issue with **child** issues as tickets backed by beads's priority-queue mechanics — see `bd prime` for the `/wayfinder` workflow.
