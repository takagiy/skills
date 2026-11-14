---
name: delegate
description: Decides whether to hand a step to a subagent (web-searcher, editor, worker) and which one. Use when a step would bring a large amount of content into the main context that is only needed briefly, such as web research, reading long or many files, long command output, or writing large file changes.
---

# Delegate

Delegation saves tokens in the main context: a subagent reads large content and returns only the conclusion, or works out and writes large file changes itself. Starting a subagent has a fixed cost, so delegate only when it saves more than it costs.

## Whether to delegate

When the step reads:

- If it brings in a lot of content (pages, files, logs, search results) and only its conclusion is needed afterward, then delegate.
- Else (you need a large part of the raw content to decide what to do next, or the content is small), do it yourself.

When the step runs a command with long output:

- If only a small part of the output is needed, then filter it yourself with `grep`, `head`, or similar.
- Else (most of the output is needed to reach a conclusion), delegate.

When the step writes:

- If a one-line command such as `sed` or `perl -pi` can make the change, then do it yourself.
- Else if the change requires writing a lot of text, then delegate.
- Else (the change is small), do it yourself.

## Which agent

- If the step is finding information on the web, then use `web-searcher`.
- Else if the step reads local files to return information, then use `editor`.
- Else if the step changes local files, then use `editor`.
- Else (it needs skills, or mixes shell, web, and files), use `worker`.

## How to delegate

- Pass the goal, the paths or URLs, the constraints, the checks to pass, and what to return.
- Ask for only what the next step needs, such as a short answer, a list of paths, or a summary of changes.
- If steps are independent, then start their subagents in parallel.
- If the result falls short, then continue the same subagent with SendMessage instead of redoing the work in the main context.
