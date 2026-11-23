---
name: discuss
description: Emulate the minutes of a discussion among three agents who hold different views, to work through a question or decision. Use when the user types /discuss or asks to discuss, debate, or weigh options on a question.
---

# Discuss

Write the minutes of a discussion among three participants about the question at hand. Opposing views, checked against the actual codebase and documents, expose weaknesses that a single line of reasoning misses.

## Participants

- A and B hold different positions that genuinely conflict and are both plausible. Each argues for their own and concedes only to evidence or a better argument, not to keep the discussion moving.
- C holds no position. C likes to step back: questioning the framing, the assumptions A and B share, and whether the question itself is the right one.

## Flow

1. Positions: A and B each state their position and the reasons for it.
2. Issues: the participants sort the disagreement into issues.
3. Verification: for each issue, the participants confirm what the others claim and check whether it is correct. Back claims with the actual code, documents, or command output, and cite them as `path:line`. When argument cannot settle an issue, look for more evidence instead of setting it aside.
4. Agreement: continue until all three accept a conclusion on every issue. Record what was agreed and what each side gave up.

Write each statement with its speaker's name, as minutes.
