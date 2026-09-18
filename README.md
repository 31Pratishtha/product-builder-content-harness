# Product Builder Content Harness

This repository is the source of truth for how our team turns product-building work into useful public content.

The harness combines:

- stable brand context;
- audience hypotheses;
- platform-specific rules;
- repeatable workflows;
- evaluation rubrics;
- human review;
- evidence-based memory.

## What this repository is for

We use it to turn ideas, build logs, product decisions, failures, user research, and source material into content for LinkedIn, X, and eventually long-form platforms.

We are not trying to automate publishing or remove human judgment. We are trying to make good thinking reusable and make the path from experience to publishable content more reliable.

## Current operating loop

1. Copy `templates/content-brief.md` or `templates/source-record.md` into `inputs/inbox/`.
2. Fill every required field. Mark unknowns explicitly.
3. Ask Codex to run the relevant workflow in `workflows/`.
4. Review the generated pack in `outputs/drafts/<content-id>/`.
5. Record edits and decisions using `templates/human-review.md`.
6. Copy accepted final variants to `outputs/approved/<content-id>/<platform>/`, preserving drafts and evaluations.
7. After manual publishing, save exact public text and performance records in `outputs/published/<content-id>/<platform>/`.
8. Run `workflows/learn-from-feedback.md` weekly.

## Non-negotiables

- Human review is required before publishing.
- The harness must not invent experience, results, users, quotes, or certainty.
- One observation is not a durable rule.
- Published copy is preserved exactly; do not overwrite history.
- Brand and workflow changes must cite the evidence that motivated them.

## Initial platforms

LinkedIn and X are active. Long-form is experimental and should be generated only when requested.

## Getting started

The brand and project context are initial working hypotheses. Voice examples illustrate style; they are not evidence of team experience.

Before calibration, record two real pieces made through the team's normal process in `experiments/baseline/`, including time, major edits, reviewer scores, and final copy. Baselines, pilot runs, publishing, learning reviews, and teammate invitations are still pending.

Fill a brief in `inputs/inbox/`, then ask the agent:

```text
Run workflows/idea-to-content-pack.md using inputs/inbox/<content-id>.md.
Generate only the requested platforms and use supported claims.
Write the pack to outputs/drafts/<content-id>/ and leave canonical files unchanged.
```

Replace `<content-id>` with the actual brief ID. For substantial sources, use `workflows/source-to-content-pack.md` instead. These are agent instructions, not executable commands or automated access controls.

See `VALIDATION.md` for scaffold checks and documented clarifications. The original implementation plan is retained unchanged as background; the scaffold includes the agreed clarifications.
