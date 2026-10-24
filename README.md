# .github — org-wide defaults

GitHub uses the files in this repository as **defaults for every repository in the org** that does not define its own.

| Path | Purpose |
|---|---|
| `profile/README.md` | Org landing page (github.com/project-templates-org) |
| `ISSUE_TEMPLATE/` | Issue forms: Epic, Feature, Task, Bug. Each form sets the org **issue type** automatically |
| `ISSUE_TEMPLATE/config.yml` | Disables blank issues, links to support & security |
| `pull_request_template.md` | Default PR description |
| `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md` | Community health files |
| `workflow-templates/` | Starter workflows shown under **Actions → New workflow → By project-templates-org** |

## Rules

- A repository that adds its own `.github/ISSUE_TEMPLATE/` (or any of these files) **replaces** the default for that file type — keep one source of truth here unless a repo really needs something different.
- This repository must stay **public** for the defaults to apply to public repositories.
- Changes go through PRs to `main`.
