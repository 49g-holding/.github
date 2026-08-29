# Recommended branch protection

Recommended settings for `main` in every `49g-holding` repository, including this one. An org owner applies them in the GitHub UI (**Settings → Rules → Rulesets**, or classic **Settings → Branches**); the scoped tokens used by tooling cannot set them.

## Baseline — every repository

- Require a pull request before merging; no direct pushes to `main`.
- Required approving reviews: 1. While the organization has a single active maintainer, allow repository administrators to bypass, so the maintainer can merge their own pull requests once checks pass; the bypass is removed when the first non-founder human joins (sunset trigger).
- Block force pushes to `main`.
- Block deletion of `main`.
- Require conversation resolution before merging.

## Once CI exists in a repository

- Require status checks to pass before merging.
- Require branches to be up to date before merging.

## As the team grows

- Require review from Code Owners (`CODEOWNERS`).
- Require signed commits.
- Move per-repository rules into organization-level rulesets.
