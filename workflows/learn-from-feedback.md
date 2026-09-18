# Workflow: Learn from Feedback

## Frequency

Run weekly after at least one item has received human review or audience feedback.

## Inputs

- human reviews from the period;
- published final versions;
- performance records;
- qualitative comments or conversations;
- memory candidates from generation runs;
- relevant rejected drafts.

## Procedure

1. Compare generated drafts with human-edited versions.
2. Group edits by reason: factual, voice, structure, clarity, usefulness, platform fit, confidentiality, or taste.
3. Identify repeated patterns. Do not generalize from one weak signal.
4. For each proposed learning, record:
   - evidence;
   - number of supporting instances;
   - possible alternative explanation;
   - confidence: low, medium, or high;
   - proposed destination file;
   - proposed exact change.
5. A learning is eligible for human-approved promotion only when:
   - it appears in at least three independent instances; or
   - one instance reveals a serious factual, ethical, legal, confidentiality, or reputational risk; or
   - a human explicitly makes a durable editorial decision.
6. Prefer adding a narrow rule over rewriting the brand broadly.
7. Write proposals to `experiments/runs/<review-id>/learning-review.md`, including evidence, exact proposed edits, and pending decisions. Use a new review ID if the directory exists. Stop for explicit human approval before changing durable memory or canonical rules; eligibility alone is not approval.
8. After approval, record the reviewer, date, accepted/rejected/deferred outcome, and reason in the review. Add accepted changes to `memory/learnings.md` and `memory/decisions.md`, and apply only explicitly approved brand, platform, workflow, or evaluation changes. Submit durable changes through a GitHub pull request for review.
9. Record the harness change in `CHANGELOG.md`.

## Important distinction

Low performance does not automatically mean poor content. Consider topic, timing, distribution, audience size, format, and sample size before changing a rule.
