# project-templates-org

Reusable templates for running software projects on GitHub: repositories, branching, reviews, CI guards and project boards.

| Start here | What it is |
|---|---|
| [`project-template`](https://github.com/project-templates-org/project-template) | Template repository — click **Use this template**, then run `scripts/bootstrap.sh` |
| [Project Template board](https://github.com/orgs/project-templates-org/projects) | Template project board (Epic → Feature/Task/Bug, iterations, roadmap) — copied for each new project |
| [`.github`](https://github.com/project-templates-org/.github) | Org-wide issue forms, PR template, contributing & security policy |

**Flow:** `feature/*` → `development` → `staging` → `main` · releases are tagged `vX.Y.Z` and backed up as read-only `release/vX.Y.Z` branches.
