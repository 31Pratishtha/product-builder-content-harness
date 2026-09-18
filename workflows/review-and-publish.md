# Workflow: Review and Publish

## Purpose

Turn a generated draft into a factually approved, voice-aligned final artifact while preserving the human decisions that matter.

## Human review sequence

1. Factual check: Is every claim supportable?
2. Confidentiality check: Is any employer, customer, team, or product information unsafe to publish?
3. Voice check: Does this sound like something we would genuinely say?
4. Usefulness check: What will the intended reader understand or do differently?
5. Platform check: Does the structure fit how the platform is read?
6. Taste check: Are we proud to attach our names to it?

## Outcomes

- `approve`: no material changes needed;
- `approve-with-edits`: human edits are required and recorded;
- `revise`: return once with specific reasons;
- `reject`: preserve the draft and record why;
- `hold`: good material, wrong timing or insufficient evidence.

## On approval

- Review each platform independently in `human-review.md`, identifying the chosen variant, reviewer, date, edits, and outcome. A held or rejected X draft does not block an approved LinkedIn draft.
- For `approve-with-edits`, apply and record the edits and obtain human confirmation of the exact final copy before treating it as ready to publish.
- Copy the exact final copy to `outputs/approved/<content-id>/<platform>/content.md` and its completed review to `human-review.md` in that platform directory.
- Preserve the original draft and evaluation.
- Complete `human-review.md`.
- Only after a human reports actual publication, copy the exact public text to `outputs/published/<content-id>/<platform>/content.md`, copy the completed review there, and record URL, platform, and publication date in `performance.md` from `templates/performance-record.md`.
- Keep published `content.md` immutable. For subsequent measurement windows, create `performance-<captured-at>-<measurement-window>.md` beside it using the same template; never replace an earlier measurement. A correction to published text needs a separately identified record linked to the original.
- If an approved or published target already exists, stop and ask for a new revision identifier rather than overwrite it.

The harness must never publish automatically in v0.1.
