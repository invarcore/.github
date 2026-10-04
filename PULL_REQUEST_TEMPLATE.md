## Description
<!-- Provide a brief summary of the changes introduced by this pull request. -->

## Motivation & Context
<!-- Why is this change required? What issue does it fix? Link relevant issue numbers. -->

## Type of Change
- [ ] 🐛 Bug fix (non-breaking change which fixes an issue)
- [ ] ✨ New feature (non-breaking change which adds functionality)
- [ ] 💥 Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] 📝 Documentation update
- [ ] ⚡ Performance optimization / refactor

## Verification & Quality Checklist
- [ ] **100% Offline Testing**: Unit tests run without external network calls, live API keys, or live HTTP requests.
- [ ] **Deterministic Fixtures**: Any new test corpora are checked into `tests/fixtures/corpora/`.
- [ ] **Test Coverage**: Maintained or increased existing test coverage threshold ($\ge 90\%$).
- [ ] **Lint & Style**: Passed `flake8` / `black` formatting checks.
- [ ] **Zero Secrets**: Verified no API keys, private tokens, or credentials are included in commit diffs.
