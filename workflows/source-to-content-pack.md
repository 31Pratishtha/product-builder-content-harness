# Workflow: Source to Content Pack

## Use when

The input contains a transcript, article, meeting note, build log, research note, product document, or other substantial source.

## Required context

Read:

- `brand/vision.md`
- `brand/values-and-beliefs.md`
- `brand/audience.md`
- `brand/voice.md`
- `brand/claims-and-boundaries.md`
- `strategy/content-pillars.md`
- `strategy/topic-rules.md`
- the platform files requested by the input
- all evaluation rubrics

Read relevant approved or rejected examples only when the input requests them or the voice is ambiguous.

## Procedure

1. Validate required metadata and source evidence under `AGENTS.md`. Return `blocked-needs-input` with specific questions when incomplete. Check the content ID is unused before writing.
2. Extract facts, observations, results, hypotheses, opinions, examples, and unresolved questions.
3. Identify confidential, unsupported, or ambiguous material.
4. Score candidate topics using `strategy/topic-rules.md`.
5. Produce three distinct angles. For each, name:
   - target audience;
   - central promise;
   - supporting evidence;
   - why it fits now;
   - risk or missing evidence.
6. Select one recommended angle and explain the selection in no more than 150 words.
7. Generate platform-specific drafts only for requested platforms.
8. Evaluate every generated variant against the quality, voice, and platform-fit rubrics, identifying variant names and failed passages in `evaluation.md`.
9. Revise once if a hard gate fails, preserving the original variant, then re-evaluate. Flag remaining failures or unmet score thresholds as `needs-human-decision`.
10. Create memory candidates, but do not update memory.

## Output directory

Write to `outputs/drafts/<content-id>/`:

- `source-analysis.md`
- `angle-options.md`
- `linkedin.md` when requested
- `x.md` when requested
- `longform.md` when requested
- `evaluation.md`
- `human-review.md`, copied from the template
- `memory-candidates.md`

Record input references, content ID, requested platforms, and harness commit or version in `source-analysis.md`. In `human-review.md`, create a separate pending review section for each requested platform. Generation never supplies human approval.

## Stop conditions

Return `blocked-needs-input` instead of drafting when:

- the central experience or claim is unclear;
- a necessary source is missing;
- confidential information cannot be separated safely;
- the requested point requires invented evidence.
