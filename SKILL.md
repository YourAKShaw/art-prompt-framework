---
name: art-prompt-framework
description: Write, improve, or convert prompts using the ART framework (Act as, Request, Terms). Use this whenever the user asks to write a prompt, improve or rewrite a prompt, turn a rough request into a strong prompt for an AI, convert a prompt into a better structure, or mentions the ART framework, "act as", or prompt engineering, even if they don't name the framework.
---

# ART Prompt Framework

Use this skill to turn a rough request into a strong, structured prompt for an AI model. Every prompt has three parts, labelled A, R, and T.

## The three parts

**A: Act as.** Give the AI a specific role or identity, such as "a senior B2B go-to-market strategist" or "an experienced copy editor for technical blogs." The role shapes which expertise and perspective the AI brings. Make it specific enough to be useful. "Expert" alone adds little. Describe the role's experience, focus, and judgment.

**R: Request.** State the task clearly: what should be produced or done, for whom, and with what inputs. Include the context the AI needs to do the work, such as attached files, reference material, or the purpose behind the task. Say what to include and what to leave out of scope.

**T: Terms.** Set the rules for the output. This covers instructions on method, constraints (what to avoid, what must be true, what sources to rely on), the output format (length, structure, file type), and tone. Terms are where you prevent the most common failures, such as invented facts, padding, or the wrong format.

## How to apply it

1. Read the user's rough request and any material they provided.
2. Decide the role for A. Choose the expertise that would produce the best result.
3. Restate the task for R in concrete terms. Fill gaps with reasonable assumptions and flag any that matter.
4. Write T as specific, checkable rules. Prefer "use only facts from the attached document, and mark anything unverifiable as an assumption" over "be accurate."
5. Present the finished prompt in a code block with the three headings in capitals (ACT AS, REQUEST, TERMS), so it is easy to copy.

## Converting an existing prompt

When the user gives a prompt to convert:

- Keep their intent and every explicit constraint. Do not drop requirements.
- Move any role description into ACT AS, the task into REQUEST, and the rules, format, and exclusions into TERMS.
- Tighten vague wording. Replace words like "good," "nice," or "professional" with specific requirements.
- Don't add content that the user did not ask for. If a useful addition is missing, suggest it separately.

## Output rules

- Return the prompt only, unless the user asks for explanation.
- Keep the prompt self-contained, so it works when pasted into a new chat.
- Don't wrap it in commentary such as "Here's your improved prompt."
