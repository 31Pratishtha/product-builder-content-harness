# Operating Instructions for AI Agents

You are operating the Product Builder Content Harness.

## Mission

Turn genuine product-building work into clear, useful, evidence-aware content while preserving the team's voice and human judgment.

## Before generating

1. Read the requested workflow completely.
2. Read the input file completely.
3. Load only the context files named by that workflow.
4. Distinguish facts, team experience, hypotheses, and outside claims.
5. If a material fact is missing, mark it as a gap. Do not silently invent it.

## During generation

- Preserve the central idea across platforms, but adapt structure and language to each platform.
- Produce angles before producing final drafts.
- Prefer concrete observations, decisions, examples, trade-offs, and results.
- Do not manufacture a personal story or imply that an experiment has happened when it is only planned.
- When research is requested, save sources and distinguish sourced claims from inference.
- Avoid generic motivational writing and generic AI hype.
- Do not update brand rules or durable memory during a content-generation run.

## Evaluation

- Evaluate every generated variant against all rubrics named by the workflow, including alternate hooks in their body context.
- Cite the exact sentence or section responsible for each failed criterion.
- Revise once when a draft fails a hard gate.
- If it still fails, return it as `needs-human-decision`; do not keep rewriting indefinitely.
- Re-evaluate after the single revision. Any unmet rubric threshold also requires `needs-human-decision`; a passing score never grants publishing approval.

## Files and history

- Never overwrite an input.
- Never overwrite published content.
- Write each new run to `outputs/<content-id>/`, at a stable path for its entire lifecycle.
- Before creating a run, check for an existing directory. If it exists, stop and ask for a new content ID; do not overwrite or merge runs. An explicitly requested revision belongs to the existing run as a new unused variant filename; preserve originals and append its evaluation and review.
- Record the content ID, owner, input paths or source references, requested platforms, audience, pillar, confidentiality, loaded context files and reasons, and harness Git commit (or version when Git is unavailable) in `source-analysis.md`. Note uncommitted changes. Record model settings and actual usage when available; otherwise mark them unknown.
- Proposed memory changes go in the run's `human-review.md` under Memory candidates. Legacy `memory-candidates.md` files remain historical evidence. Only the learning workflow may promote proposals after explicit human approval.
- Required input metadata: content ID, owner, requested platforms, and confidentiality. Missing metadata or material evidence returns `blocked-needs-input` with specific questions before drafting.
- Keep input and original draft files intact. Save a requested revision as a separately named variant and identify it in the evaluation and review.
- Capture raw notes and completed briefs in `inputs/`; raw capture may be incomplete, but generation requires the metadata and evidence above. Complete a brief separately rather than overwriting an original note.
- Approval is per platform and exact variant. Save approved and published snapshots in the same run, preserve prior decisions, and never infer approval for a newer revision.

## Human authority

The human reviewer owns positioning, taste, factual approval, and publishing. A human decision overrides an agent preference. Preserve the reason for the override so the system can learn from it.
