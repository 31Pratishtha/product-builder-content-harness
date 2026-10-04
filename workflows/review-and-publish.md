# Workflow: Review and Publish

## Context

Read AGENTS.md, the run's source-analysis.md, relevant sources, all variants being considered, evaluation.md, human-review.md, and the applicable brand/platform guidance. Load templates/performance-record.md only when recording publication or performance.

## Human review

Review factual support, confidentiality, voice, usefulness, platform fit, and taste. Record each platform independently in human-review.md with reviewer, date, selected variant, material edits and reasons.

Outcomes: approve, approve-with-edits, revise, reject, or hold. A held X draft does not block an approved LinkedIn draft. Generation and rubric scores cannot supply human approval.

## Revisions and approval

- Preserve original drafts and review decisions. Append dated review entries instead of replacing prior decisions.
- Save a requested revision as <platform>-v<N>.md using the next unused number; evaluate it under workflows/generate-content.md.
- For approve-with-edits, apply edits to a separately named variant, record them, evaluate the resulting variant, and obtain human confirmation of its exact final copy.
- After explicit approval, copy the exact chosen text to outputs/<content-id>/<platform>-approved-v<N>.md. Record that path and the source variant in the review.
- Approval attaches to that exact copy; later revisions require their own review.
- If any target filename exists, stop for a new revision identifier. Never overwrite draft, approved, or published snapshots.

## Publication and measurement

- Publishing remains manual. Only after a human reports actual publication, save the exact public text as outputs/<content-id>/<platform>-published-v<N>.md.
- Record publication URL, date, platform, approved snapshot, and published snapshot in a dated review entry. If the public text differs, preserve that fact and obtain factual review of the actual version; do not infer approval from an earlier variant.
- Use templates/performance-record.md to create performance-<platform>-<captured-at>-<measurement-window>.md in the same run. Record only observed results.
- Each later measurement gets a new filename. Keep published text immutable; any correction needs a new identified snapshot linked to its predecessor.
- Keep feedback beside the content it concerns. Do not duplicate reviews into separate status folders.
