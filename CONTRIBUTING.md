# Contributing to Invarcore

Thank you for your interest in contributing to Invarcore! We welcome contributions that help advance reliable, verifiable, and secure autonomous systems.

---

## 1. Development Principles

### The Fundamental Rule: Offline Deterministic Testing
* **Zero Live HTTP in Unit CI**: Unit tests must run 100% offline without live network dependencies (`curl`, `requests.get("https://...")`, or live API keys).
* **Two-Tier Architecture**:
  * **Tier 1 (Golden Fixtures)**: Public benchmark corpora checked into `tests/fixtures/corpora/`. Evaluated in every pull request; guaranteed sub-second and deterministic.
  * **Tier 2 (Live Integration)**: Opt-in integration harness executed via script flags (e.g. `--fetch-live-corpus`).
* Any unit test that fails due to network latency, DNS resolution, or rate limiting will block the pull request.

---

## 2. Pull Request Workflow

1. **Fork & Branch**: Create a feature branch with a descriptive name:
   * `feat/<feature-name>` for new capabilities
   * `fix/<bug-name>` for bug fixes
   * `docs/<topic>` for documentation improvements
2. **Quality Gates**: Ensure code passes formatting, type checking, and tests:
   ```bash
   pytest
   flake8
   ```
3. **Test Coverage**: PRs must maintain or improve repository test coverage ($\ge 90\%$).
4. **Commit Hygiene**: We enforce **Conventional Commits**:
   * `feat: add SlidingWindowStreamBuffer to canary engine`
   * `fix: correct HMAC payload ordering during validation`
   * `docs: update quickstart guide for local deployment`
   * `test: add golden fixture for NIST SP 800-53 evaluation`

---

## 3. Code of Conduct

We are committed to providing a welcoming, constructive, and harassment-free community for everyone. Be respectful, constructive, and open to feedback.
