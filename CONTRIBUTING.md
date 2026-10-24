# Contributing

These rules apply to every repository in **project-templates-org** unless a repository ships its own `CONTRIBUTING.md`.

## 1. Start from an issue

1. Every change starts with an issue: **Epic**, **Feature**, **Task** or **Bug** (pick the matching form).
2. Large work is an **Epic**; break it down with **Create sub-issue**.
3. The issue is triaged on the project board: Priority, Size, Iteration, Status = `Ready`.
4. Assign yourself and move the item to `In progress` when you start.

## 2. Branch

Branch from `development` (or from `main` for a hotfix):

| Prefix | Use for | Base / PR target |
|---|---|---|
| `feature/<issue>-<slug>` | new functionality | `development` |
| `fix/<issue>-<slug>` | non-urgent bug fix | `development` |
| `chore/`, `docs/`, `refactor/`, `test/`, `ci/`, `perf/`, `build/` | maintenance | `development` |
| `hotfix/<issue>-<slug>` | urgent production fix | from `main` → PR to `main` |

Example: `feature/42-sso-login`.

Promotion is always by pull request: `development` → `staging` → `main`.
Full details: [branching strategy](https://github.com/project-templates-org/project-template/blob/main/docs/branching-strategy.md).

## 3. Commit & PR

- PR titles follow [Conventional Commits](https://www.conventionalcommits.org): `feat(auth): add SSO login`.
- Feature PRs are **squash-merged**, so the PR title becomes the commit message.
- Promotions and back-merges use **merge commits** (keeps branch history shared, avoids repeat conflicts).
- Link the issue: `Refs #42` (or `Closes #42` for PRs into `main`).
- Keep PRs small (< 400 changed lines where possible). Draft PRs are welcome for early feedback.

## 4. Review

- Required checks must pass: `branch-flow`, `pr-title`, `ci`.
- `staging` and `main` require 1 approval (org admins may bypass in emergencies; record why in the PR).
- Reviewers: be specific, label nits as `nit:`, approve when it is good enough, not perfect.

## 5. Definition of done

- Acceptance criteria met, tests pass, docs updated.
- Merged to `development` → Status `In staging` once promoted → `Done` once in `main` / released.
