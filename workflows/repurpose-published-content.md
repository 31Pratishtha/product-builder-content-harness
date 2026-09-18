# Workflow: Repurpose Published Content

## Use when

A human-approved published piece should be adapted to another platform or format.

## Rule

Repurposing means preserving the underlying idea and evidence while redesigning the presentation for a different reader behavior. It does not mean shortening or expanding sentence by sentence.

## Procedure

Read the required context listed in `workflows/source-to-content-pack.md`, using the destination platforms. Require the metadata defined in `AGENTS.md`; ask specific questions and return `blocked-needs-input` for missing metadata, sources, reviews, or material evidence.

1. Read the exact published source and its human review.
2. Identify the central claim, strongest evidence, best example, and reader promise.
3. Read the destination platform file.
4. Choose the best native format for that platform.
5. Draft the new version without adding unsupported facts or experiences.
6. Evaluate every variant for platform fit, quality, and voice. Revise once after a hard-gate failure, preserve the original, and re-evaluate. Flag any remaining failures or unmet thresholds as `needs-human-decision`.
7. Write a note describing what was preserved, removed, and reframed.

## Output

Create a new unused content ID linked to the original. Do not overwrite the published source. Use the pack filenames and traceability fields in `workflows/source-to-content-pack.md`; record adaptation reasoning in `source-analysis.md`, considered native angles in `angle-options.md`, and any memory proposals in `memory-candidates.md`. Include separate pending human reviews for each destination platform.
