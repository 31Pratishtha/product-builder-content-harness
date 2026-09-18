# Workflow: Idea to Content Pack

## Use when

The input is an original idea, question, observation, or rough note rather than a substantial external source.

## Required context

Read the same brand, strategy, platform, and evaluation files required by `workflows/source-to-content-pack.md`.

## Procedure

1. Validate required metadata and material evidence under `AGENTS.md`, returning `blocked-needs-input` with specific questions when incomplete. Check the content ID is unused, then restate the idea in one precise sentence.
2. Identify the first-hand experience or reasoning that supports it.
3. List missing facts or evidence.
4. Decide whether the idea is:
   - ready to draft;
   - ready only as a question or hypothesis;
   - in need of research;
   - too generic to pursue.
5. If research is needed and authorized, gather it and create a source record. Otherwise stop with specific research questions.
6. Create three angles and score them using `strategy/topic-rules.md`.
7. Select one recommended angle.
8. Generate requested platform drafts.
9. Evaluate every generated variant. Revise once after a hard-gate failure, preserving the original, then re-evaluate. Mark remaining failures or unmet score thresholds `needs-human-decision`.
10. Create memory candidates without changing durable memory.

## Output

Use the output directory, filenames, traceability fields, and separate pending platform reviews defined in `workflows/source-to-content-pack.md`.
