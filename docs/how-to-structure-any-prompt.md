### PROMPT

A prompt is an instruction set. The clearer the instruction, the better the result.

Five parts. You will not use all five every time. But knowing them means you always know which one is missing when the output is not right.

1. Indentity, tell agent who he is right now, not that necesarry for coding already covered by CLAUDE/AGENT.md
2. Task - what needs to get done
Be specific. "Help me write something" is vague. "Write a 200-word product description for [X] targeting [Y] audience" gives Claude something to work with.
Good tasks have three things:
- A clear action — write, review, analyze, compare, build, fix, summarize
- A defined scope — how long, how many, what format, what section
- Enough detail that someone unfamiliar with your project could attempt it
3. Context - What agent needs to know:

This is the background. The constraints. The audience. Prior decisions. Relevant data. Anything Claude needs to do the task well that it would not know on its own.

If you are using a CONTEXT.md, that should handle the project-level stuff. But for individual prompts, you can also give context directly:
example:
```
We are a 15-person startup. Our customers are mid-market HR directors. We just launched a feature that automates onboarding checklists. Here is the feature spec: [paste spec]
```
Guessing is where AI outputs go sideways

4. Constrainst - What should agent avoid?

Telling agent what you do NOT want is just as useful as telling it what you do want.
example:

> Do not use jargon. Write at an 8th grade reading level.

> Do not suggest solutions that require a paid API. Everything should use free tools.

> Keep it under 300 words. No bullet points. Write in paragraphs.

> Do not start with "In today's world" or any variation of it.

5. Output format - What should the result look like?

Tell agent the shape of the answer. A list? A table? Three options to choose from? A code block with comments? A draft with placeholder sections?

> Give me three headline options, each under 10 words, followed by a one-sentence explanation of the angle.

> Return this as a markdown table with columns for Task, Owner, Deadline, and Status.

> Write the first draft with [PLACEHOLDER] wherever I need to fill in company-specific details.

> Give me the answer as a numbered list, then add a one-paragraph summary at the end.

For coding sometimes the output can be a pattern, a code block, a list of commands, etc.

note: Task and Constraints live in your prompts. Identity and Context live in your files.

## Chunking: breaking big projects into prompts

The rule: each prompt should ask for one clear thing.