# Security policy

## Reporting a vulnerability

**Do not open a public issue.**

Use GitHub's private reporting: open the affected repository → **Security** → **Report a vulnerability**.
Private vulnerability reporting is enabled on all repositories. Include:

- affected repository, version / commit
- description and impact
- steps to reproduce or proof of concept

We aim to acknowledge reports within **3 business days** and to provide a remediation plan within **10 business days**.

## Supported versions

Only the latest release on `main` receives security fixes unless a repository states otherwise.

## Practices in this org

- Secret scanning and push protection are enabled on repositories.
- Dependabot alerts and security updates are enabled.
- Never commit secrets — use GitHub Actions **secrets** / **environments**.
