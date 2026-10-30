<div align="center">

# 🎨 ART Prompt Framework

[![AgentShield Security](https://merx.help/badge/A+.svg)](https://merx.help/shield)

[![HOL Guard](https://img.shields.io/endpoint?url=https%3A%2F%2Fhol.org%2Fapi%2Fregistry%2Fbadges%2Fplugin%3Fslug%3Dyourakshaw%252Fart-prompt-framework%26metric%3Drelease)](https://hol.org/registry/plugins/yourakshaw%2Fart-prompt-framework)

**🚀 Stop prompting like it's 2023!** A systematic framework and agent skill for engineering sharp, reliable AI prompts.

Turn vague one-liners into structured, context-rich prompts that get the best out of modern LLMs. Drop it in, say *"make this a prompt,"* and watch the magic happen 🪄🔥

---

[![GitHub Tag](https://img.shields.io/github/v/tag/YourAKShaw/art-prompt-framework?label=version&style=for-the-badge&logo=git&color=2563EB)](https://github.com/YourAKShaw/art-prompt-framework/tags)
[![License: MIT](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Claude Skill Ready](https://img.shields.io/badge/Claude-Skill%20Ready-7C3AED?style=for-the-badge&logo=anthropic&logoColor=white)](https://claude.ai)
[![Agent Skills](https://img.shields.io/badge/Agent-Skills-F97316?style=for-the-badge&logo=githubcopilot&logoColor=white)](https://skills.sh)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-059669?style=for-the-badge&logo=github)](https://github.com/YourAKShaw/art-prompt-framework/pulls)
[![GitHub Stars](https://img.shields.io/github/stars/YourAKShaw/art-prompt-framework?style=for-the-badge&logo=github&color=F59E0B)](https://github.com/YourAKShaw/art-prompt-framework/stargazers)
[![Issues](https://img.shields.io/github/issues/YourAKShaw/art-prompt-framework?style=for-the-badge&logo=github&color=EF4444)](https://github.com/YourAKShaw/art-prompt-framework/issues)

</div>

---

## ⚡ Overview

Most prompt failures come from three missing ingredients: **unclear expertise**, **vague objectives**, and **absent constraints**. The **ART Framework** fixes all three with a simple tripartite structure applied to every prompt it writes or refactors:

| Component | Focus | What it does |
| :--- | :--- | :--- |
| 🎭 **A: Act As** | **Persona & Expertise** | Sets the AI's perspective, seniority, and domain authority. Replaces generic "expert" labels with a specific professional identity. |
| 🎯 **R: Request** | **Mission & Context** | Defines the deliverable, the inputs, the audience, and what is out of scope. |
| ⚖️ **T: Terms** | **Rules & Guardrails** | Sets the boundaries: format, length, tone, sources, and things to avoid. |

---

## 💡 Why ART?

- 🎯 **Fewer invented facts**: Explicit terms and negative constraints keep the output anchored to what you actually gave it.
- ⚡ **Copy-paste ready**: Every output is a self-contained block that works in a brand-new chat.
- 🧩 **Works beyond Claude**: The skill is a single `SKILL.md` file. The prompts it writes are plain text, so they run in any LLM.
- 🔬 **Repeatable results**: Replaces trial-and-error prompting with a structure you can reuse and improve.

---

## 🔍 The Anatomy of an ART Prompt

Here is how a one-line request becomes an actionable ART prompt:

### ❌ The Rough Input
> *"Help me write a cold email to a SaaS founder."*

### ✅ The Generated ART Prompt
```markdown
ACT AS:
A seasoned B2B sales copywriter who writes short, specific cold emails
that busy SaaS founders actually read.

REQUEST:
Write one cold email to the founder of a 20-person B2B SaaS company that
sells inventory software to small retailers. Goal: book a 15-minute call.
Use only the company name and the founder's first name as placeholders.

TERMS:
1. Length: 75 to 100 words.
2. Tone: direct, peer-to-peer. No buzzwords, no exclamation marks,
   no "I hope this finds you well."
3. Structure:
   - Line 1: one specific observation about the company (no generic praise).
   - Line 2: the value, with one concrete benefit.
   - Line 3: one low-friction call to action.
4. Do not invent facts about the company. If something is unknown, leave it out.
```

---

## 📥 Installation

### 🛠️ Claude Code (Personal Skill)

Clone the repository into your personal skills directory:

```bash
git clone https://github.com/YourAKShaw/art-prompt-framework.git ~/.claude/skills/art-prompt-framework
```

### 📦 Skills CLI (Other Agents)

```bash
npx skills add YourAKShaw/art-prompt-framework
```

### 🌐 Claude.ai (Web App)

1. Download this repository as a [ZIP archive](https://github.com/YourAKShaw/art-prompt-framework/archive/refs/heads/main.zip).
2. Make sure `SKILL.md` is at the root of the extracted folder.
3. Upload the folder or ZIP via **Claude Settings → Capabilities / Skills**.

---

## 🚀 Usage

Once installed, ask your agent to write, improve, or convert a prompt, or mention the ART framework by name:

### ✍️ Prompt Creation
> *"Write an ART prompt to help me build an automated financial reconciliation pipeline in Python."*

### 🔧 Prompt Refactoring
> *"Turn this into a strong prompt using the ART framework: 'Create a system design document for a real-time chat application.'"*

The skill returns a clean, self-contained prompt in a code block, ready to paste into a new chat.

---

## 🧭 Compatibility

| Environment | Status |
| :--- | :--- |
| 🛠️ Claude Code | ✅ Supported |
| 🌐 Claude.ai | ✅ Supported |
| 📦 Other agents (via Skills CLI) | 🧪 Check your agent's docs for where skills are loaded |

---

## 📂 Repository Layout

```text
art-prompt-framework/
├── 📜 SKILL.md      # The skill: framework, conversion rules, output rules
├── ⚙️ .github/     # Commit message workflow and checker
├── 📘 README.md     # Project documentation
├── 🔒 SECURITY.md   # Vulnerability reporting policy
├── ⚖️ LICENSE       # MIT License
└── 🛡️ .gitignore   # Git ignore rules
```

---

## 🤝 Contributing

Contributions, feedback, and new prompt patterns are warmly welcomed! 🙌

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/new-prompt-pattern`).
3. Commit your changes (`git commit -m 'feat: add new terms template'`).
4. Push to the branch (`git push origin feature/new-prompt-pattern`).
5. Open a Pull Request.

For a large change to the framework itself, open an issue first so we can agree on the approach.

---

## 🔒 Security

Found a vulnerability? Please report it privately as described in [`SECURITY.md`](SECURITY.md) instead of opening a public issue.

---

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for full details.
