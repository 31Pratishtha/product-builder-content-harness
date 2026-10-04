# Initial Content Experiment

## Goal

Determine whether the harness can produce publishable content that sounds like us, preserves factual integrity, and reduces repeated effort.

## Duration

Four weeks or 10 published content packs, whichever takes longer.

## Active platforms

- LinkedIn: primary platform.
- X: secondary platform for concise ideas, threads, and conversation.
- Long-form: generated only for a source with enough depth and only when requested.

## Content mix

- 4 build or decision logs;
- 2 failure or changed-mind analyses;
- 2 harness engineering explainers grounded in our implementation;
- 2 reusable artifacts or frameworks.

## Baseline

Before relying on the harness, create two pieces through the team's normal process and record:

- minutes from idea to reviewable draft;
- number of major edits;
- reviewer voice score;
- reviewer usefulness score;
- confidence in factual accuracy.

## Harness success measures

- median time to a reviewable content pack;
- percentage of drafts accepted after one human review;
- average voice-rubric score;
- average quality-rubric score;
- factual or unsupported-claim failures;
- major edit categories;
- number of published pieces;
- meaningful replies, saves, profile visits, conversations, or inbound interest.

Engagement is diagnostic, not the only measure of quality. Do not optimize for impressions alone.

## Decision after the experiment

Choose one:

- continue with the current structure;
- revise context or workflows;
- narrow the brand or audience;
- automate a repeated mechanical step;
- stop the experiment if the process creates more overhead than value.

## Records and comparisons

Create records only when work is performed; do not create empty baseline or results directories. Save manual baselines as `evals/baseline-<id>.md`, reusable cases as `evals/case-<id>.md`, and comparisons as `evals/result-<id>.md`. Use unused IDs and preserve earlier measurements.

Cases should include complete evidence, incomplete metadata, unsupported claims, conflicting sources, confidentiality, repurposing, and independent platform approvals. Record expected behavior and human scoring criteria before comparing outputs.

Compare the same inputs using the normal process, a simple prompt baseline, and the harness. Record model/settings, harness version and uncommitted changes, loaded context, reviewer edits, time to approval, and actual token/cost data when exposed. Mark unavailable measurements unknown. Repeat comparisons when variability could change the conclusion; retain all attempts rather than selecting only the best.

Report hard-gate failures separately from editorial scores. Measure time and cost per approved piece, including failed attempts. Use relevant cases to check changes to prompts, workflows, context selection, and models before adopting them. These records assess quality and efficiency; rubric scores never grant publication approval.
