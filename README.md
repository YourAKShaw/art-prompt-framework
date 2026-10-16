# ART Prompt Framework

A simple Claude skill for writing, improving, and converting AI prompts using the **ART** structure:

- **A: Act as.** The role or expertise the AI should adopt.
- **R: Request.** The task, its inputs, and its purpose.
- **T: Terms.** The rules, constraints, output format, and tone.

## Install

### Claude Code (personal skill)

```bash
git clone https://github.com/<your-username>/art-prompt-framework.git ~/.claude/skills/art-prompt-framework
```

### Claude.ai

Download this repository as a ZIP, rename the extracted folder to `art-prompt-framework` if needed, and upload it through the skills settings. Make sure `SKILL.md` sits at the top level of the folder.

## Usage

Ask Claude to write, improve, or convert a prompt, or mention the ART framework by name. Example:

> Turn this into a strong prompt using the ART framework: "help me write a cold email to a SaaS founder."

Claude returns the prompt in a code block with ACT AS, REQUEST, and TERMS headings.

## Repository layout

```
art-prompt-framework/
├── SKILL.md      # The skill itself (required)
├── README.md     # This file
├── LICENSE       # MIT license
└── .gitignore
```

## License

MIT. See [LICENSE](LICENSE).
