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
- Write each run into its own content-ID directory.
- Before writing, check for an existing run directory. If it exists, stop and ask for a new content ID; do not overwrite or merge runs.
- Record the content ID, input paths or source references, requested platforms, and harness Git commit (or version when Git is unavailable) in `source-analysis.md`.
- Proposed memory changes go into the run's `memory-candidates.md`; only the weekly learning workflow may promote them after explicit human approval.
- Required input metadata: content ID, owner, requested platforms, and confidentiality. Missing metadata or material evidence returns `blocked-needs-input` with specific questions before drafting.
- Keep input and original draft files intact. Save a requested revision as a separately named variant and identify it in the evaluation and review.

## Human authority

The human reviewer owns positioning, taste, factual approval, and publishing. A human decision overrides an agent preference. Preserve the reason for the override so the system can learn from it.
