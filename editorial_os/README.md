# KARTIK . H — LinkedIn Editorial OS

An adapted integration of selected LinkedIn Agent Skill workflows, designed to extend—not replace—Kartik's established editorial system.

## What this is

This package provides:
- A ChatGPT project-instruction supplement and reusable workflow prompts.
- A Claude Code skill pack with matching editorial rules.
- A shared editorial constitution so both environments produce consistent work.

It is an editorial assistant, not a publishing bot. It drafts, critiques, structures, and analyses. Kartik reviews and publishes manually.

## Order of authority

This package is tooling. It sits under the repository's own documents and does not replace them:

1. `02_EDITORIAL_CONSTITUTION.md` — the writing standard.
2. `04_ESSAY_INDEX.md` — what the series publishes next, and the quality test.
3. `01_KNOWLEDGE_MAP.md` — the canonical domain list.
4. This package — workflows that apply the above.

Where this package and those documents disagree, those documents win. See `INTEGRATION.md`.

## Non-negotiable editorial hierarchy

1. Factual integrity and evidence
2. Credibility and professional positioning
3. Original insight and systems understanding
4. Clarity and usefulness
5. Memorability
6. Engagement

Reach, hooks, formatting, and engagement metrics never override the hierarchy above.

## Included workflows

| Workflow | Purpose |
|---|---|
| `linkedin-post` | Develop a thoughtful post from a raw idea, source, observation, achievement, or builder log |
| `linkedin-comment` | Write substantive comments that add context, a mechanism, evidence, or a useful question |
| `linkedin-reply` | Respond to comments while preserving tone and building genuine professional dialogue |
| `linkedin-profile-audit` | Review profile positioning for a student-founder / healthcare systems builder, not a generic sales profile |
| `linkedin-content-audit` | Review content performance using relevant quantitative and qualitative signals |
| `linkedin-weekly-plan` | Plan around the established Tuesday/Friday cadence without forcing volume |
| `linkedin-human-review` | Conduct a final editorial quality check; no AI-detector score chasing |
| `linkedin-repurpose` | Adapt an existing idea across formats without repeating or diluting it |

## Installation

### ChatGPT

1. Open the `chatgpt/` folder.
2. Add `PROJECT_INSTRUCTIONS_SUPPLEMENT.md` to this project's instructions, or paste it into the project instruction field after your existing rules.
3. Keep `EDITORIAL_CONSTITUTION.md` as the shared reference.
4. Use prompts from `WORKFLOW_PROMPTS.md` when invoking a workflow.

The instructions are also usable directly in this current ChatGPT project. They do not require a connector, API key, or LinkedIn login.

### Claude Code

1. Copy the `.claude/` directory into the root of the project/repository where you use Claude Code, or copy its `skills/` directory into your user-level `~/.claude/skills/` directory.
2. The skills are invoked by their names, for example `/linkedin-post` or `/linkedin-comment`.
3. Copy `reference/EDITORIAL_CONSTITUTION.md` to a stable location and update the `@` reference in each skill if you choose a different path. By default, each skill contains the core rules inline so it remains portable.

Claude Code skill discovery can vary by version and configuration. If a skill does not appear, verify that its folder contains `SKILL.md` and restart/reload the Claude Code session.

## What was deliberately changed from the source repository's approach

- The generic 4-post-per-week plan is replaced with the user's established Tuesday/Friday cadence.
- The profile rubric is rewritten from a service-sales lens to a credible student-founder / healthcare knowledge systems lens.
- Hook formulas are optional tools, not the starting point or the goal.
- Humanizer/detector scoring is not used as a measure of authenticity or AI detection. Only concrete copy-editing checks are retained.
- Algorithm claims about outbound links, dwell time, or ranking weights are not repeated as facts without current reliable evidence.
- Comments, replies, and DMs must be genuine, specific, and non-manipulative. No engagement bait, mass outreach, or auto-send.
- All publishing remains under human control.

## Safety and scope

- Never invent metrics, citations, awards, patient outcomes, clinical claims, quotations, credentials, or product capabilities.
- Distinguish user-provided experience, verified source evidence, inference, and uncertainty.
- Do not expose patient-identifiable, confidential, or sensitive information.
- For healthcare content, do not convert educational discussion into individualized diagnosis, prescribing, or treatment advice.
- Do not fabricate engagement metrics or infer audience sentiment from a small sample.

## Versioning

Version: 1.0 — adapted editorial integration.

This package does not install itself into ChatGPT or Claude, modify account settings, or connect to LinkedIn. It supplies portable instructions and skills for the user to install where desired.
