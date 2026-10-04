# Security Policy

Invarcore develops zero-trust, governance-critical, and verification-focused infrastructure for autonomous AI systems. We treat all security vulnerabilities with the highest priority.

---

## Supported Versions

We provide security updates and patches for the following versions:

| Repository / Engine | Active Version | Security Support |
| :--- | :--- | :--- |
| **`canary-fabric`** | `v0.2.x` | :white_check_mark: Supported |
| **`intent-fabric`** | `v0.1.x` | :white_check_mark: Supported |
| **`knowledge-fabric`** | `v0.1.x` | :white_check_mark: Supported |
| **`enterprise-adapters`** | `v0.1.x` | :white_check_mark: Supported |
| **`unloop`** | `v0.1.x` | :white_check_mark: Supported |
| **`cachealign`** | `v0.1.x` | :white_check_mark: Supported |

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues or discussions.**

To report a vulnerability privately, use one of the following methods:

1. **GitHub Private Vulnerability Reporting (Preferred)**:
   * Navigate to the **Security** tab of the relevant Invarcore repository.
   * Click **Report a vulnerability** to open an encrypted private advisory with the maintainers.

2. **Direct Maintainer Contact**:
   * Email: `security@invarcore.com` (or contact maintainer [@sagarv48](https://github.com/sagarv48)).
   * Include detailed reproduction steps, proof-of-concept payloads, and affected versions.

---

## Response Timeline & Disclosure Process

* **Initial Response**: Within 24–48 hours confirming receipt of the advisory.
* **Triage & Assessment**: Severity and impact evaluated based on CVSS scoring within 3 business days.
* **Fix & Release**: Coordinated patch developed in a private security fork.
* **Public Disclosure**: A security advisory and CVE (if applicable) will be published alongside the patched release.

---

## Scope & Bounties

In-scope items include:
* Canary token evasion or HMAC forgery in `canary-fabric`
* Unchecked state execution or policy bypass in `intent-fabric`
* Secret scrubbing / DLP bypass in `enterprise-adapters`
* Cache poisoning or prefix desynchronization in `cachealign`
* Memory exhaustion or denial-of-service in trajectory recording in `unloop`
