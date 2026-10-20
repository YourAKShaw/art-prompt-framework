# 🛡️ Security Policy

## 📌 Supported Versions

Security fixes are made on the `main` branch and shipped in the next tagged release. Only the latest release receives fixes.

| Version | Supported |
| :--- | :--- |
| Latest release (`v1.x`) | ✅ |
| Older releases | ❌ |

## 🎯 Scope

This project is an agent skill made of plain-text instructions (`SKILL.md`). It runs no code of its own, but a flaw in its instructions can still cause harm. Examples of issues in scope:

- Instructions that could lead an agent to leak secrets, credentials, or private files.
- Instructions that could be abused for prompt injection or to make an agent ignore the user's intent.
- Anything in the repository that could cause an agent to run unsafe commands.

Out of scope: vulnerabilities in Claude, other AI models, agent runtimes, or the Skills CLI. Report those to their maintainers.

## 🔒 Reporting a Vulnerability

**Please do not open a public issue for security problems.**

Report privately through GitHub's [private vulnerability reporting](https://github.com/YourAKShaw/art-prompt-framework/security/advisories/new). Include:

1. A description of the issue and its impact.
2. Steps or a prompt that reproduce it.
3. The version or commit you tested.

## ⏱️ Response Times

- **Acknowledgement:** within 3 business days.
- **Initial assessment:** within 7 days.
- **Fix or mitigation:** as soon as possible, usually within 30 days for confirmed issues.

You will be kept informed of progress and credited in the release notes unless you prefer to stay anonymous.
