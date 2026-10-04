# Invarcore Organization Meta Repository (`.github`)

This repository serves as the central configuration and governance repository for the [Invarcore](https://github.com/invarcore) organization.

---

## What Lives Here

1. **Organization Profile (`profile/README.md`)**:
   * Renders as the public landing page for the organization at [github.com/invarcore](https://github.com/invarcore).
2. **Organization-Wide Community Health Files**:
   * `SECURITY.md`: Central security and vulnerability disclosure policy applied across all Invarcore repositories.
   * `CODEOWNERS`: Default code ownership and review assignments.
   * `CONTRIBUTING.md`: Engineering standards, two-tier test isolation requirements, and commit conventions.
   * `PULL_REQUEST_TEMPLATE.md`: Standard quality and verification checklist for PRs.
   * `ISSUE_TEMPLATE/`: Standardized bug report and feature request templates.
3. **Branding Assets (`assets/`)**:
   * Official logos, emblems, and visual assets for Invarcore.

---

## Repository Structure

```
.github/
├── assets/
│   ├── invarcore-logo-with-text.jpg   # Primary logo lockup
│   └── invarcore-logo-emblem.jpg      # Minimalist emblem
├── profile/
│   └── README.md                      # Organization landing page
├── ISSUE_TEMPLATE/
│   ├── bug_report.md
│   ├── feature_request.md
│   └── config.yml
├── CODEOWNERS
├── CONTRIBUTING.md
├── PULL_REQUEST_TEMPLATE.md
├── README.md
└── SECURITY.md
```
