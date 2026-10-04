# Scaffold Validation

## Current structure — 2026-09-27

The user approved implementation of the proposed ten-directory redesign. Existing uncommitted content and prior changelog history were preserved.

### Migration map

| Historical location | Current location |
| --- | --- |
| brainstorms/2026-09-22-product-psychology-and-discovery.md | inputs/2026-09-22-product-psychology-and-discovery.md |
| inputs/inbox/2026-09-22-discovery-format-research.md | inputs/2026-09-22-discovery-format-research.md |
| outputs/drafts/2026-09-22-discovery-format-research/ | outputs/2026-09-22-discovery-format-research/ |
| strategy/experiment-plan.md | evals/pilot-plan.md |
| workflows/idea-to-content-pack.md | workflows/generate-content.md (idea branch) |
| workflows/source-to-content-pack.md | workflows/generate-content.md (source branch) |
| workflows/repurpose-published-content.md | workflows/generate-content.md (repurpose branch) |

Existing input and output text was preserved byte for byte during migration, including draft filenames, sources, evaluation, review, and memory candidates. References inside those historical artifacts resolve through this map; they are not instructions to recreate obsolete folders. The original implementation plan and the September 18 report below document the earlier layout.

New runs use versioned platform drafts. The existing run retains linkedin.md, x.md, and longform.md so its original evaluation and review references stay meaningful.

Empty placeholders and the empty decision-map run directory were removed. No approved or published content existed in the removed status folders. Unused memory log templates were removed after confirming they held no operational entries; existing decisions remain preserved.

### Validation scope

Migration checks compare file hashes and inspect current workflow references, directory layout, collision rules, versioned revisions, per-platform approval, and learning approval requirements. These are structural checks, not an executed content pilot. Quality, voice calibration, token savings, publication, and audience outcomes still require real runs.

Completed checks: all migrated files matched their pre-move SHA-256 hashes before guidance edits; all 15 historical run artifacts and both inputs remain present; the ten expected main directories exist; 27 active guidance files have no missing static file references or obsolete operational paths; git diff --check passed. Historical references in preserved content and earlier reports intentionally remain documented by the migration map.

## Historical scaffold report — 2026-09-18

Date: 2026-09-18

## Delivery status

The local Content Harness v0.1 scaffold is complete. This is a Markdown operating system, not an application or an automated enforcement layer. Baselines, real content runs, human editorial reviews, publishing, and learning outcomes have not been performed or fabricated.

The existing GitHub repository is linked through SSH as `origin`. SSH access succeeded and the remote initially contained no refs. GitHub reported public visibility, contrary to the agreed private setup; pushing is pending resolution of that difference. Commit, tag, and remote verification are reported in the implementation handoff.

## Created files

34 specified Markdown files:

- Root: `README.md`, `AGENTS.md`, `CHANGELOG.md`.
- Brand: `brand/vision.md`, `brand/values-and-beliefs.md`, `brand/audience.md`, `brand/voice.md`, `brand/claims-and-boundaries.md`.
- Strategy: `strategy/content-pillars.md`, `strategy/topic-rules.md`, `strategy/experiment-plan.md`.
- Platforms: `platforms/linkedin.md`, `platforms/x.md`, `platforms/longform.md`.
- Workflows: `workflows/source-to-content-pack.md`, `workflows/idea-to-content-pack.md`, `workflows/repurpose-published-content.md`, `workflows/review-and-publish.md`, `workflows/learn-from-feedback.md`.
- Templates: `templates/content-brief.md`, `templates/source-record.md`, `templates/human-review.md`, `templates/performance-record.md`.
- Evaluation: `evals/quality-rubric.md`, `evals/voice-rubric.md`, `evals/platform-fit.md`.
- Knowledge: `knowledge/product-building-initiative.md`, `knowledge/glossary.md`.
- Memory: `memory/README.md`, `memory/decisions.md`, `memory/feedback-log.md`, `memory/learnings.md`, `memory/wins.md`, `memory/failures.md`.

11 `.gitkeep` files preserve empty directories: `knowledge/examples/approved/`, `knowledge/examples/rejected/`, `knowledge/references/`, `inputs/inbox/`, `inputs/active/`, `inputs/processed/`, `outputs/drafts/`, `outputs/approved/`, `outputs/published/`, `experiments/baseline/`, and `experiments/runs/`.

Also added `.gitignore` and this report. A later update added `brainstorms/README.md` for pre-brief idea capture. The supplied implementation document remains unchanged.

## Checks performed

- Extracted all 34 initial Markdown blocks directly from the supplied document. All specified files exist; 21 match the initial text and 13 contain the documented clarifications below (comparison normalizes line endings and trailing whitespace).
- All explicit static workflow path references resolve. Requested platform files, three evaluation rubrics, input templates, and inherited source-workflow context exist.
- Paths containing content IDs, platforms, review IDs, or measurement windows are future run artifacts, not missing scaffold files. Pack-local filenames are generated by the named workflows. No run artifacts are required during setup.
- All 11 placeholder directories exist and contain no invented examples or operational results.
- `git check-ignore --no-index` confirms representative environment files, credentials, private keys, editor settings, and temporary files are ignored. Representative inbox, draft, published, and baseline Markdown paths remain trackable.
- No application code, external dependencies, publishing automation, or persistent test tools were added.

## Hypothetical workflow walkthroughs

These are document-level checks, not executed model runs or evidence of content quality.

| Scenario | Expected instruction path | Review result |
| --- | --- | --- |
| Complete idea requests LinkedIn and X | Generate angles and platform variants, evaluate each, create two pending platform reviews | Covered by idea/source workflows and agent rules |
| Source lacks owner or requested platforms | Return `blocked-needs-input` with specific questions before drafting | Covered by source template and agent rules |
| Source would require invented experience | Stop; do not generate a personal story | Covered by source stop conditions and claims boundaries |
| A variant fails a hard gate twice or misses score thresholds | Preserve variants; return `needs-human-decision` after the bounded revision | Covered by all generation workflows |
| LinkedIn approved while X is held | Copy only the selected approved LinkedIn final; preserve both drafts | Covered by platform review and publishing workflow |
| Approval requires edits | Record edits and obtain confirmation of exact final copy | Covered by publishing workflow |
| Repurpose a published piece | New content ID, source link, full context, evaluations, pending destination reviews | Covered by repurposing workflow |
| Existing run or publication path | Stop for a new identifier; preserve existing history | Covered by agent and publishing rules |
| Later performance measurement | New dated measurement record; public text stays unchanged | Covered by publishing workflow |
| Three supporting learning instances | Proposal is eligible, but durable files stay unchanged until human approval | Covered by learning workflow and memory policy |
| No real publication or human review supplied | Leave operational records empty and decisions pending | Covered by setup scope and review rules |

## Intentional deviations from supplied initial text

- `README.md`: copy rather than move drafts; per-platform storage; first-run directions; working-hypothesis and pending-baseline notes.
- `AGENTS.md`: required metadata, collisions, run provenance, preserved revisions, all-variant evaluation, unmet thresholds, and explicit approval for memory promotion.
- `CHANGELOG.md`: records these initial workflow clarifications.
- `brand/voice.md`: marks examples as illustrative rather than verified experience.
- Source and idea workflows: required metadata, provenance, independent reviews, variant evaluation, and bounded revision handling.
- Repurposing workflow: explicit inherited context and complete pack outputs with source linkage.
- Publishing workflow: independent approval, exact final-copy confirmation, platform directories, immutable published text, and separate performance snapshots.
- Learning workflow: persisted proposals and human decisions before any durable changes; reviewed pull requests for durable changes.
- Content brief and source templates: required metadata and explicit confirmation of confidentiality; source template gains content ID, owner, platforms, and confidentiality.
- Human-review template: repeatable per-platform review sections instead of one pack-wide outcome.
- `memory/README.md`: evidence eligibility does not replace human approval.

## Remaining operational work

Resolve repository visibility and verify the pushed branch/tag. Teammate invitations are deferred. Record two manual baselines before calibration; then supply real inputs, complete reviews, publish manually, and conduct the first learning review. The original plan's full operational definition of done remains pending.

Rubrics and human gates are procedural instructions. Scaffold validation cannot prove that a model will obey them or that the outputs will match the team's voice. Those require real runs and human assessment.
