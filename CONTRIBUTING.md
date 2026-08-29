# Contributing

These conventions apply to repositories in the `49g-holding` organization unless a repository defines its own `CONTRIBUTING.md`. The full engineering rulebook lives in the `49g-standards` repository and governs where the two overlap.

## Language

All repository surfaces — commit messages, issues, pull requests, reviews, documentation — are written in English.

## Branches and commits

- `main` is protected: changes land through pull requests, not direct pushes (see `docs/BRANCH_PROTECTION.md`).
- Branch names: `feat/<topic>`, `fix/<topic>`, `docs/<topic>`, `chore/<topic>`.
- Commit subjects: imperative mood, at most 72 characters; add a body when the change needs context.

## Pull requests

- Every pull request states what changed and why, and links the issue it closes when one exists.
- One approving review before merge. While the organization has a single active maintainer, the maintainer may merge their own pull request after checks pass; this rule tightens as the team grows.

## Issues

Use the provided templates. Never file security problems as issues — see `SECURITY.md`.

## Credentials

No credentials, tokens, private keys, or personal data are ever committed — to any repository, in any form, including in history. A leaked secret is rotated immediately and reported to the organization owners.
