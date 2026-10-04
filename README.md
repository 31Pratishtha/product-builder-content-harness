# Product Builder Content Harness

Turn genuine product-building work into useful public content with evidence, a consistent voice, and human judgment.

## Structure

| Location | Responsibility |
| --- | --- |
| AGENTS.md | Shared operating rules, evidence gates, and history protection |
| brand/ | Audience, identity, values, voice, and claim boundaries |
| strategy/ | Content pillars and topic selection |
| knowledge/ | Reusable facts about our products and team |
| platforms/ | Guidance for requested destinations |
| workflows/ | Generation, review, and approved learning |
| templates/ | Reusable briefs, source records, reviews, and measurements |
| evals/ | Rubrics, pilot plan, and real evaluation records |
| inputs/ | Original brainstorms, briefs, transcripts, and source notes |
| outputs/ | One stable directory per content ID |
| memory/ | Learning policy, approved decision history, and dated learning reviews |

## Operating loop

1. Capture a dated note in `inputs/`. Raw brainstorms may be incomplete; identify new notes with `input_type: brainstorm`.
2. For generation, create a new brief using `templates/content-brief.md` or `templates/source-record.md`. Link the original note and preserve it. Require content ID, owner, requested platforms, confidentiality, and adequate evidence.
3. Run `workflows/generate-content.md` with the input path.
4. Review `outputs/<content-id>/human-review.md`. Each platform has its own decision and exact selected variant.
5. Use `workflows/review-and-publish.md` to save approved and actually published snapshots beside the drafts.
6. Record audience feedback and dated performance measurements in the same run.
7. Use `workflows/learn-from-feedback.md` to propose durable changes. Apply them only after explicit human approval.

Files stay at stable paths. Review status belongs in the run's human review; do not move inputs or outputs between status directories.

## Start a run

```text
Run workflows/generate-content.md using inputs/<dated-input>.md.
Generate only the requested platforms using supported claims.
Write a new pack to outputs/<content-id>/.
```

Idea, substantial source, and repurposing inputs use the same workflow with different evidence checks. LinkedIn and X are active when requested; long-form is opt-in.

## Context and evaluation

The workflow defines context by stage. Read only relevant knowledge and requested platform guidance. Read referenced sources completely; do not replace evidence with an unsupported summary. Record the files actually loaded in source-analysis.md. Stable file storage does not itself guarantee lower token use.

Use `evals/pilot-plan.md` for the initial pilot. Record two manual baselines as `evals/baseline-<id>.md` when they are performed. Add real regression cases and results as dated files under evals; create subdirectories only when their volume requires them. No baseline or publishing results are implied by the scaffold.

The files are agent instructions, not executable enforcement. Humans own factual approval, positioning, taste, and publication.

## Migrated history

See `VALIDATION.md` for the September 27 migration and old-to-new path mapping. Existing inputs and run artifacts retain their original text and filenames, including historical path references and the original memory-candidates.md. New runs use versioned draft filenames and review-local proposals.

The supplied implementation plan and earlier changelog entries describe previous versions and remain historical references.
