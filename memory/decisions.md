# Editorial and Harness Decisions

## D-005 — Context before the method, natural progression

- Date and reviewer: 2026-10-04, Pratishtha.
- Decision: Apply the user's explicit preference for context, useful storytelling, natural transitions, and avoiding cliches or unnecessary instructions to future drafts and voice checks.
- Reason: Earlier rubric passes missed tone problems the reviewer identified, including the second X opening.
- Evidence: outputs/2026-09-22-discovery-format-research/human-review.md; memory/learning-review-2026-10-04-natural-voice.md.
- Destinations: brand/voice.md, evals/voice-rubric.md, evals/case-voice-context.md, workflows/generate-content.md.
- Scope: editorial preference across platforms; no invented stories, mandatory narrative template, or audience-performance claim.
- Confidence: high on the stated preference; effect on unseen drafts remains untested.
- Review date: after the next three distinct content runs, or earlier on human correction.

## D-004 — Stable content paths and consolidated feedback

- Date: 2026-09-27
- Decision: Use ten purpose-specific directories, one stable output directory per content ID, a unified generation workflow, and feedback stored with the affected content.
- Approval: The user explicitly requested implementation of the folder redesign in this task.
- Reason: Reduce duplicate records, path changes, and irrelevant context loading while preserving evidence and human approval.
- Scope: Repository organization and operating instructions; no change to brand positioning or content approval.
- Evidence: Current workflow overlap and unused status/experiment folders inspected during the redesign; see VALIDATION.md for migration details.
- Destinations: README.md, AGENTS.md, workflows/, templates/, evals/pilot-plan.md, memory/README.md.
- Revisit when: Real review and pilot results identify missing context, excessive overhead, or retrieval problems.

## D-001 — Repository is the source of truth

- Date: initial version
- Decision: Keep canonical harness context and history in this Git repository.
- Reason: The team needs inspectable, versioned, shareable, and tool-independent context.
- Revisit when: A stable workflow and non-technical usage justify a dedicated application.

## D-002 — Human approval is required

- Date: initial version
- Decision: No content is published automatically in v0.1.
- Reason: The team is still discovering its voice and must protect factual accuracy, confidentiality, and taste.

## D-003 — LinkedIn and X are active first

- Date: initial version
- Decision: Generate LinkedIn and X by default when both are requested; long-form remains opt-in.
- Reason: This limits complexity while still testing cross-platform transformation.
