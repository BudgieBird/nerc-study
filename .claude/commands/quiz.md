---
description: Generate practice exam questions
---

Activate the nerc-exam skill. Generate questions based on this request: $ARGUMENTS

Read `/reference/nerc-glossary.md` and `/reference/exam-traps.md` first to ensure question accuracy.

If the request is "20" or "give me 20", use the weak-area weighting defined in the skill.
If the request is a specific topic, generate 10 questions on that topic.
If the request is "full", generate 50 questions across all domains.

After grading, log results to `/progress/daily-scores.md`.
