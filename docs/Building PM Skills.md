# Building PM Skills

This guide explains how we turn real-world PM frameworks and source materials into agent-ready skills in this repo.

## What Counts As A Skill

A skill is a reusable framework that produces a clear outcome and can be applied across companies or products.

| If it is... | Then it is... |
| --- | --- |
| A repeatable framework with a concrete output | A skill |
| One-off advice or tips | A prompt |
| Long-form context or theory | Research |

## Choose The Skill Type

Pick the smallest type that fits the job.

- Component: A single deliverable template or artifact. Use for PRD sections, user stories, statements, or canvases.
- Interactive: A guided decision flow with 3-5 questions and 3-5 numbered recommendations.
- Workflow: A multi-phase process that orchestrates other skills and includes decision points.

## Distill The Source

Use source material (posts, books, internal playbooks) to extract the minimum that makes the framework work.

- Outcome: What does the skill help produce.
- Audience: Who the output is for and what they care about.
- Steps: The smallest reliable sequence that gets to the output.
- Decisions: Key forks and what to do in each branch.
- Pitfalls: The common failure modes the framework prevents.
- Definitions: Jargon the reader might not know.
- Examples: At least one strong example and one explicit anti-pattern.

## Draft The Skill File

Create a new folder in `skills/<skill-name>/SKILL.md` with lowercase kebab-case naming. Every skill must use the standard section order and frontmatter fields.

```markdown
---
name: skill-name
description: One-line description that includes when to use it
type: component
---

## Purpose

## Key Concepts

## Application

## Examples

## Common Pitfalls

## References
```

## Quality Bar

- Keep language opinionated and practical.
- Use short paragraphs and concrete instructions.
- Include a clear example and an explicit anti-pattern.
- Define jargon on first use.
- Make tradeoffs explicit.

## Example: Substack Post To Product Demo Skill

Assume the source is a post about demo regret and stage fright. The goal is to help PMs design a demo that lands with the audience and avoids common traps.

**Decision:** This is likely a workflow if you want multi-phase execution (briefing, narrative, rehearsal, contingency). If you only want a short Q and A flow that outputs a demo outline, make it interactive.

Sample workflow frontmatter and structure:

```markdown
---
name: product-demo
description: Plan and run product demos that land with the audience, avoid demo regret, and include rehearsal and contingency planning. Use when preparing a demo for stakeholders, customers, or executives.
type: workflow
---

## Purpose
Define the demo goal, anchor the story to the audience, and reduce risk before presenting.

## Key Concepts
- Demo regret: When a demo shows features but fails to prove value.
- Stage fright: Performance anxiety that affects delivery and clarity.
- Aha moment: The single proof point the demo must land.

## Application
1. Intake: audience, goal, time, decision at stake.
2. Narrative: problem, constraint, proof, payoff.
3. Flow: 5-7 minute core path, optional branches.
4. Rehearsal: 2 dry runs, one with interruptions.
5. Contingency: offline backup, screenshots, and failure plan.

## Examples
- Good: 8-minute enterprise demo that anchors on a single outcome and shows proof in the first 2 minutes.
- Anti-pattern: Feature tour with no stated decision or success criterion.

## Common Pitfalls
- Overstuffed flow that can only succeed if the demo is perfect.
- No backup path when the system fails.

## References
- Stage fright is real. So is product demo regret. (source post)
```

## Repo Checklist

- Add the skill under `skills/<skill-name>/SKILL.md` with correct frontmatter.
- Update the catalog counts and tables in `README.md`.
- Link related skills where appropriate.
- Run a quick scan with `rg "<skill-name>"` to ensure references are correct.
