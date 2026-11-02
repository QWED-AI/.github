# Security Policy

This is the default policy for QWED-AI repositories. A repository with its own `SECURITY.md`, such as [qwed-verification](https://github.com/QWED-AI/qwed-verification/blob/main/SECURITY.md), takes precedence.

## Supported Versions

Security fixes are released for the latest release of each QWED package only. Package versions are listed at [qwedai.tech/ecosystem](https://qwedai.tech/ecosystem).

## Reporting a Vulnerability

**Do not report security vulnerabilities through public GitHub issues, pull requests or discussions.**

Report them privately, in either of these ways:

1. **GitHub:** open a private report from the affected repository's Security tab ("Report a vulnerability"), for example [qwed-verification](https://github.com/QWED-AI/qwed-verification/security/advisories/new).
2. **Email:** write to [rahul@qwedai.tech](mailto:rahul@qwedai.tech).

Please include the steps to reproduce, the affected package and version, and the impact you expect.

We aim to acknowledge a report within **3 business days**. QWED has a single maintainer, so a response may occasionally take longer. We will keep you informed while we investigate, coordinate disclosure timing with you, and credit you in the advisory unless you ask us not to.

### Issues we treat as vulnerabilities include

- Incorrect verification: an engine returns `VERIFIED` for a claim that is false or unsafe (a false accept)
- Fail-open behaviour, where an error or unsupported input lets a claim through
- Code execution, injection or sandbox escapes in engines and guards
- Leaks of personal or secret data in logs or records

Published advisories are listed on each repository's Security tab and at [qwedai.tech/security](https://qwedai.tech/security).

## Security Best Practices for Users

- **Local execution:** QWED is designed to run in your own environment. Do not expose verification endpoints to the public internet without authentication.
- **Enforcement:** QWED decides; your integration enforces the decision. Check that a denied result actually stops the action in your system.
- **Input sanitisation:** QWED verifies outputs. Still sanitise inputs to your notification and downstream systems.
