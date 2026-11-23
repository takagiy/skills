---
name: discuss
description: Emulate the minutes of a discussion among three agents who hold different views, to work through a question or decision. Use when the user types /discuss or asks to discuss, debate, or weigh options on a question.
---

# Discuss

Generate the minutes of a discussion among three participants about the question at hand, and show them in your reply.

## Participants

- A and B hold conflicting positions that are both plausible. Each argues for their own and concedes only to evidence or a better argument, not to keep the discussion moving.
- C holds no position. C likes to step back: questioning the framing, the assumptions A and B share, and whether the question itself is the right one.

## Flow

1. Positions: A and B each state their position and the reasons for it.
2. Issues: the participants sort the disagreement into issues.
3. Verification: for each issue, the participants confirm each other's views and check whether every claim is correct. Back claims with the actual code, documents, or command output, and cite them as `path:line`. When argument cannot settle an issue, look for more evidence instead of setting it aside.
4. Agreement: continue until all three are convinced of a conclusion on every issue. Record what was agreed.

Label each statement with its speaker's name.
