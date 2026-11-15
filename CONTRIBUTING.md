# Contributing to QWED

Thank you for your interest in contributing to QWED! We are building the verification infrastructure for the AI era, and we welcome contributions from the community.

## 🤝 How to Contribute

### 1. Reporting Bugs
- **Search First:** Check [Issues](https://github.com/issues?q=is%3Aissue+is%3Aopen+org%3AQWED-AI) to see if the bug is already reported.
- **Use the Template:** Open a new issue using the **Bug Report** template.
- **Reproduce:** Provide a minimal reproduction script or steps.

### 2. Suggesting Features
- **Discuss First:** Open a [Discussion](https://github.com/orgs/QWED-AI/discussions) to gauge interest and refine the idea.
- **RFC Process:** Significant changes require a Request for Comments (RFC) issue.

### 3. Pull Requests
- **Fork & Branch:** Fork the repo and create a branch like `feat/new-guard` or `fix/logic-error`.
- **Tests:** Add unit tests for your changes. We aim for >90% coverage.
- **Linting:** Ensure your code passes our linting checks (ruff/black/mypy).
- **Commit Messages:** Use [Conventional Commits](https://www.conventionalcommits.org/) (e.g., `feat: add logic guard`, `fix: overflow error`).
- **PR Template:** Fill out the PR template completely.

## 🛠️ Development Setup

Most QWED repositories follow this setup:

```bash
# Clone the repo
git clone https://github.com/QWED-AI/qwed-verification.git
cd qwed-verification

# Create venv
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dev dependencies
pip install -e ".[dev]"

# Run tests
pytest
```

## 📜 Code of Conduct

We are committed to providing a friendly, safe, and welcoming environment for all. Please be respectful and professional in all interactions.

## 📝 License

Unless a repository's LICENSE file says otherwise, QWED repositories are licensed under the Apache License 2.0, and contributions are accepted under the same licence:

- **Inbound = outbound.** Under section 5 of the Apache License, a contribution you submit for inclusion is licensed under it, with no additional terms, unless you explicitly state otherwise.
- **You keep your copyright.** The licence lets everyone, the maintainer included, use, change and redistribute your contribution. Under section 3 you also grant a patent licence, limited to the patent claims you can license that your contribution necessarily infringes, alone or combined with the project you contribute to.
- **Only submit what you have the right to submit:** your own work, or code under a licence that is compatible with Apache-2.0, with its notices kept. Code under the GPL, the AGPL or another licence that is not compatible cannot be accepted.
- **The names are not licensed.** See the [QWED name and logo policy](https://github.com/QWED-AI/qwed-verification/blob/main/TRADEMARKS.md). Where a repository has a NOTICE file, redistributions keep it; the licence lists its other conditions.
