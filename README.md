### Agent specific markdown files

This is a template and custom rules for project context and AGENT markdown to improve claude context window and token efficiency

CLAUDE.md is a special file that Claude reads at the start of every conversation. Include Bash commands, code style, and workflow rules. This gives Claude persistent context it can’t infer from code alone.

CLAUDE.md is loaded every session, so only include things that apply broadly. For domain knowledge or workflows that are only relevant sometimes, use skills instead.

## What to include in CLAUDE.md

| ✅ Include | ❌ Exclude |
| --- | --- |
| Bash commands Claude can’t guess | Anything Claude can figure out by reading code |
| Code style rules that differ from defaults | Standard language conventions Claude already knows |
| Testing instructions and preferred test runners | Detailed API documentation (link to docs instead) |
| Repository etiquette (branch naming, PR conventions) | Information that changes frequently |
| Architectural decisions specific to your project | Long explanations or tutorials |
| Developer environment quirks (required env vars) | File-by-file descriptions of the codebase |
| Common gotchas or non-obvious behaviors | Self-evident practices like “write clean code” |

CLAUDE.md cannot be any longer than 200 lines

## 3 files
A working folder that changes how Claude responds to you. Three files. Five minutes. You will see the difference immediately.
(CLAUDE.md, CONTEXT.md, REFERENCES.md)