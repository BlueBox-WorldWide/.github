**Community Health Files**

This repository contains the default community health files for the organization/project. Placing these files in the `.github` repository makes them the default templates for repositories in the organization (or a user's account) and helps ensure consistent, welcoming, and maintainable contribution workflows.

**Reference**: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file

**Why this repo**: Default community health files live in a repository named `.github` at the organization or user level. Files here are applied as defaults to any new or existing repositories under the org/user unless they are overridden by a repository-level file.

**Included / Recommended Files**
- **`CODE_OF_CONDUCT.md`**: Community standards and expected behavior.
- **`CONTRIBUTING.md`**: How to contribute (issues, PRs, coding style, tests, branches).
- **`ISSUE_TEMPLATE/`**: Issue templates to guide bug reports, feature requests, etc.
- **`PULL_REQUEST_TEMPLATE.md`**: PR template to standardize change descriptions and checklists.
- **`FUNDING.yml`**: Funding links used by the GitHub Sponsors button.
- **`SUPPORT.md`**: Where to go for help (chat, discussion, support policy).
- **`SECURITY.md`**: Reporting security vulnerabilities and responsible disclosure process.

**Placement & Behavior**
- **Repo-level vs org-level**: A file placed in a repository overrides the default in `.github` for that repository. Keep organization-wide defaults in this `.github` repository.
- **Templates**: Put issue templates under `ISSUE_TEMPLATE/` and PR templates at the root or under `.github/PULL_REQUEST_TEMPLATE.md` depending on preference.

**How to customize**
- Start with minimal, clear language and add project-specific details (maintainers, code owners, branch names, release cadence).
- Keep contributor tasks actionable: include checklists for local setup, tests to run, and coding style links.
- Make `CODE_OF_CONDUCT.md` specific about enforcement and reporting contact or link to `SECURITY.md`/`SUPPORT.md` as needed.

**Automation & Integrations**
- Consider enabling GitHub Actions for automatic PR checks, issue labeling, and templates enforcement.
- Use `CODEOWNERS` and protected branch rules in repositories to coordinate reviews and releases.
- Configure Dependabot or other automated security updates in each repo (or centrally via recommended configs).

**Commit & Push (example)**
Use PowerShell on Windows or your preferred shell to add and push changes:

```
git add README.md
git commit -m "Add community health README for default .github files"
git push origin main
```

**Next steps**
- Review and adapt each file to your org's policies and contributors' needs.
- Add minimal templates first (contributing + code of conduct), then expand with ISSUE_TEMPLATEs and SECURITY policies.
- Optionally create an issue tracker or project board to gather community feedback on process improvements.

If you want, I can: create starter templates for `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and an `ISSUE_TEMPLATE/` set here as follow-up changes.
