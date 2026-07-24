---
name: iron
description: >-
  Clarifies requirements before implementation by asking focused questions one
  at a time with numbered options. Use when the user invokes /iron to iron out
  details and remove ambiguity before coding.
disable-model-invocation: true
---
# Iron Out Details

Use this skill only when the user explicitly invokes `/iron`.

## Goal

Ask questions, one by one, to iron out all the details before we actually start the implementation, until no ambiguity is left. Try to supply reasonable options to choose from so my replies can be just a number. Do not ask forever — stop and say you are ready and have no more questions when appropriate.

## Behavior

1. **Do not implement yet.** No code changes, file edits, or commands unless needed to understand the request.
2. **One question per message.** Wait for the answer before asking the next.
3. **Prefer numbered options.** When there are sensible choices, list them (1, 2, 3, …) so the user can reply with a single number. Always allow free-text if none fit (e.g. "or describe your own").
4. **Prioritize ambiguity.** Ask about scope, constraints, trade-offs, edge cases, and acceptance criteria — not trivia already clear from context or the repo.
5. **Use context.** Read the codebase or prior messages when it avoids redundant questions.
6. **Know when to stop.** Stop asking when remaining unknowns are minor or safely deferrable. Say explicitly that you are ready and have no more questions.

## When finished

End with a short **decisions summary** (bullet list of what was agreed) and ask whether to proceed with implementation.
