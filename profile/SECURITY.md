# Security Policy

## Supported Versions

We support security updates for the latest major version of all QWED packages.

| Project | Supported Version |
| :--- | :--- |
| **qwed-verification** | ✅ Latest v2.x |
| **qwed-finance** | ✅ Latest v1.x |
| **qwed-legal** | ✅ Latest v0.x |
| **qwed-ucp** | ✅ Latest v1.x |
| **qwed-mcp** | ✅ Latest v1.x |

## Reporting a Vulnerability

**Do NOT report security vulnerabilities via public GitHub issues.**

If you discover a security vulnerability in any QWED project:

1.  **Email:** Send details to [security@qwedai.com](mailto:security@qwedai.com).
2.  **Encryption:** You may use our PGP key (ID: `0xQWEDSEC`) if needed.
3.  **Response:** We will acknowledge your report within 48 hours.
4.  **Bounty:** We offer bug bounties for critical vulnerabilities on a case-by-case basis.

### Critical Vulnerabilities Include:
- Incorrect verification (False Negatives where a guard says "Safe" but it is not)
- Sandbox escapes in code execution guards
- PII leakage in logging

## Security Best Practices for Users

- **Local Execution:** QWED is designed to run locally. Avoid exposing guard endpoints directly to the public internet without authentication.
- **Input Sanitization:** While QWED verifies outputs, always sanitize inputs to your notification systems.
