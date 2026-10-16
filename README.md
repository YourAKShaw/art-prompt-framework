<div align="center">

# 🎨 ART Prompt Framework

**A systematic framework and Claude skill for engineering high-precision, production-grade AI prompts.**

Transform vague, one-liner requests into structured, deterministic, and context-rich prompts that unlock the full reasoning potential of modern LLMs.

---

[![GitHub Tag](https://img.shields.io/github/v/tag/YourAKShaw/art-prompt-framework?label=version&style=for-the-badge&logo=git&color=2563EB)](https://github.com/YourAKShaw/art-prompt-framework/tags)
[![License: MIT](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Claude Skill Ready](https://img.shields.io/badge/Claude-Skill%20Ready-7C3AED?style=for-the-badge&logo=anthropic&logoColor=white)](https://claude.ai)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-059669?style=for-the-badge&logo=github)](https://github.com/YourAKShaw/art-prompt-framework/pulls)
[![GitHub Stars](https://img.shields.io/github/stars/YourAKShaw/art-prompt-framework?style=for-the-badge&logo=github&color=F59E0B)](https://github.com/YourAKShaw/art-prompt-framework/stargazers)
[![Issues](https://img.shields.io/github/issues/YourAKShaw/art-prompt-framework?style=for-the-badge&logo=github&color=EF4444)](https://github.com/YourAKShaw/art-prompt-framework/issues)

</div>

---

## ⚡ Overview

Most prompt degradation stems from three missing elements: **unclear expertise**, **vague objectives**, and **absent constraints**. The **ART Framework** resolves this by enforcing a battle-tested tripartite architecture on every generated or refactored prompt:

| Component | Focus | Description |
| :--- | :--- | :--- |
| 🎭 **A — Act As** | **Persona & Expertise** | Calibrates the AI's perspective, seniority, domain authority, and cognitive standard. Replaces generic "expert" labels with nuanced professional identities. |
| 🎯 **R — Request** | **Mission & Context** | Defines the core deliverable, input data, background materials, target audience, and precise scope of work. |
| ⚖️ **T — Terms** | **Rules & Guardrails** | Establishes non-negotiable boundaries, formatting requirements, anti-hallucination guardrails, prohibited elements, and tonal guidelines. |

---

## 💡 Why ART?

- 🎯 **Eliminates Hallucination & Drift**: Explicit terms and strict negative constraints keep the model tethered to verifiable truth.
- ⚡ **Zero-Friction Reusability**: Outputs self-contained, copy-paste-ready prompt blocks that operate seamlessly in any fresh session.
- 🧩 **Model Agnostic**: Engineered natively as a Claude skill, but generates prompts equally powerful across Claude 3.5/3.7, GPT-4o, Gemini 2.5, or local open-weights models.
- 🔬 **Systematic Quality**: Replaces trial-and-error prompting with a disciplined, reproducible engineering structure.

---

## 🔍 The Anatomy of an ART Prompt

Here is how a conversational, one-line request is elevated into an actionable ART prompt:

### ❌ The Rough Input
> *"Help me write a cold email to a SaaS founder."*

### ✅ The Generated ART Prompt
```markdown
ACT AS:
A seasoned B2B enterprise sales copywriter who specializes in high-converting,
low-friction outbound email campaigns for high-growth tech founders.

REQUEST:
Draft a 3-sentence cold outreach email introducing an automated API latency
monitoring tool to a Bootstrapped SaaS Founder. Highlight immediate ROI: saving
engineering on-call hours and preventing silent churn.

TERMS:
1. Length: Exactly 75-100 words.
2. Tone: Respectful, punchy, peer-to-peer; avoid corporate fluff, sycophancy,
   and buzzwords ("synergy", "game-changer", "revolutionary").
3. Structure:
   - Line 1: Observation/context showing understanding of founder pain.
   - Line 2: Value proposition with concrete metric.
   - Line 3: Low-friction Call To Action (ask for thoughts, not a 30-min call).
4. Do not include placeholder text that requires manual editing except for
   [Recipient Name] and [Company Name].
```

---

## 📥 Installation

You can install and use the **ART Prompt Framework** directly in your preferred Claude environment:

### 🛠️ Claude Code (Personal Skill)

Clone this repository directly into your Claude personal skills directory:

```bash
git clone https://github.com/YourAKShaw/art-prompt-framework.git ~/.claude/skills/art-prompt-framework
```

### 🌐 Claude.ai (Web App)

1. Download this repository as a [ZIP archive](https://github.com/YourAKShaw/art-prompt-framework/archive/refs/heads/main.zip).
2. Ensure `SKILL.md` is positioned at the root of the extracted folder.
3. Upload the folder or zip file via **Claude Settings → Capabilities / Skills**.

---

## 🚀 Usage

Once installed, Claude automatically applies the framework whenever you want to engineer, optimize, or translate a prompt:

### Prompt Creation
> *"Write an ART prompt to help me build an automated financial reconciliation pipeline in Python."*

### Prompt Refactoring
> *"Turn this into a strong prompt using the ART framework: 'Create a system design document for a real-time chat application.' "*

Claude outputs a clean, modular prompt formatted cleanly inside a code block ready to be copied into production or another chat session.

---

## 📂 Repository Layout

```text
art-prompt-framework/
├── 📜 SKILL.md      # Core framework logic, instructions, and conversion rules
├── 📘 README.md     # Project documentation, guides, and specifications
├── ⚖️ LICENSE       # MIT License
└── 🛡️ .gitignore   # Git repository ignores
```

---

## 🤝 Contributing

Contributions, feedback, and prompt pattern enhancements are warmly welcomed!

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/new-prompt-pattern`).
3. Commit your Changes (`git commit -m 'feat: add enhanced terms template'`).
4. Push to the Branch (`git push origin feature/new-prompt-pattern`).
5. Open a Pull Request.

---

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for full details.

