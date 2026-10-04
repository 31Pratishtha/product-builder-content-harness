# Workflow: Generate Content

## Use when

Create content from an idea, substantial source, or approved published piece. Read this workflow and AGENTS.md completely before execution.

## Context by stage

- Intake and angle selection: read the input completely, brand/audience.md, brand/claims-and-boundaries.md, strategy/content-pillars.md, and strategy/topic-rules.md.
- Read knowledge/product-building-initiative.md when the topic concerns our team or product work; read knowledge/glossary.md when terminology needs clarification. Other knowledge files require a specific connection to the input.
- Drafting: also read brand/vision.md, brand/values-and-beliefs.md, brand/voice.md, and only the requested files from platforms/linkedin.md, platforms/x.md, platforms/longform.md.
- Evaluation: read evals/quality-rubric.md, evals/voice-rubric.md, and evals/platform-fit.md completely, using the draft and its evidence.
- For voice evaluation, also read evals/case-voice-context.md and check complete variants against its context and flow cases. Use the linked draft examples only when needed to resolve an ambiguous judgment; do not load the whole output history.
- Read selected prior examples and their reviews only when requested or needed to resolve voice ambiguity. Examples illustrate style; they do not establish experience for a new piece.
- Do not routinely load the pilot plan, decision history, unrelated outputs, or all knowledge. Record each file actually read and why. Do not reread unchanged context already available in the current run.

## Intake branches

Require content ID, owner, requested platforms, and confidentiality. Resolve material evidence gaps before drafting. Return blocked-needs-input with specific questions when information is missing.

- Idea or brainstorm: state the idea in one sentence, identify supporting experience or reasoning, and decide whether it is ready, supportable only as a question or hypothesis, needs research, or is too generic. Raw notes need not have metadata until generation is requested. Create a separate completed brief if needed; never overwrite the original.
- Substantial source: read the source completely and distinguish facts, observations, results, hypotheses, opinions, examples, and unresolved questions. Request missing or inaccessible source material.
- Repurpose: require the exact published text and human review, select a new content ID, and link the original. Preserve its central idea and evidence while adapting to the destination platform. Record what was preserved, removed, and reframed.

Check that outputs/<content-id>/ does not exist before creating a new run. If it exists, stop and request a new content ID. Explicit revisions to an existing run follow the separate revision rule in AGENTS.md.

## Procedure

1. Identify confidential, unsupported, or ambiguous material. Stop when the central claim requires invention or confidential evidence cannot be safely separated.
2. If research is needed and authorized, gather it and create source records using templates/source-record.md under the run's sources/ directory. Otherwise return specific research questions. Keep outside claims and our interpretation distinct.
3. Produce three distinct angles and score each using strategy/topic-rules.md. State the audience, reader promise, evidence, pillar, timely relevance, and missing evidence or risk. Do not force a piece to satisfy a pillar quota.
4. Recommend one angle with a rationale of at most 150 words.
5. Draft only requested platforms, preserving one central idea and supported claims.
6. Evaluate every variant, including alternate hooks in body context, against all three rubrics. Identify the variant, scores, hard gates, and exact failed passages.
7. After a hard-gate failure, revise once as a new version and re-evaluate. Preserve the original evaluation. Remaining hard-gate failures or unmet score thresholds require needs-human-decision; passing never grants publishing approval.
8. Copy templates/human-review.md into the run and create a pending review for each requested platform. Record any learning proposals there without changing durable rules.

## Run artifacts

Write to outputs/<content-id>/:

- source-analysis.md
- angle-options.md
- <platform>-v1.md for each requested platform
- evaluation.md
- human-review.md

In source-analysis.md record content ID, owner, input paths and source references, selected audience and pillar, requested platforms, confidentiality, evidence and gaps, context files loaded with reasons, and harness Git commit or version. Note uncommitted harness changes so a commit is not mistaken for the exact working version. Record model/settings and actual usage when available; mark unavailable metrics as unknown.

Use unused version numbers for revisions. Create sources/ only when research is collected. Do not create empty optional artifacts. Legacy runs can retain unversioned original drafts; identify those exact filenames in evaluation and review.
