# build-your-own-gadget

The meta-gadget. Designs the smallest tool that dissolves a pain — and teaches the user, by its reasoning, how to do this design move themselves.

## The problem it dissolves

> Tools for everyone.

Most people have pains they don't think of as "tool-able." The gap is not skill; it's *the move* — restating the pain, locating the latent need, naming the smallest dissolve. This gadget runs that move on demand and shows its work so the user starts running it themselves.

## How to invoke

Two inputs:

| Input | Example |
|---|---|
| **Pain** | "I keep forgetting to follow up with people I care about" |
| **Context** | "Not a developer, comfortable with copy-paste; ~2 hours a week" |

Output:
- **Restated problem** — the latent need underneath what you said
- **Who has this** — honest scope (sometimes "just me" is the right answer)
- **Smallest dissolve** — the simplest tool that solves it, fully specified
- **Evolutionary frame** — capability transfer, failure mode, after-50-uses test
- **Starter artifact** — the actual v0.1 (prompt template, script, or doc, ≤50 lines)
- **What's next** — how to extend after a few uses

## How to run

**Paste path:** open `prompt.md`, copy below the `---`, fill `{{PAIN}}` and `{{CONTEXT}}`, paste into any Claude session.

**CLI path:** `.\build-your-own-gadget.ps1 -Pain "..." -Context "..."` (needs `ANTHROPIC_API_KEY`).

## Evolutionary frame

- *Teaching surface*: the design reasoning is shown explicitly, not hidden behind a magic-feeling output
- *Capability transfer*: after a few uses, user starts seeing their own pains as solvable; the bar to try drops
- *Failure mode*: collecting tools instead of practicing the move. Refuse to deliver if the same user comes back with no application of the previous design.

## What it is NOT

- Not a code-generator. Many of its outputs are *prompts*, not scripts. The smallest dissolve is often a prompt template, not software.
- Not a guarantee. Some pains are not tool-shaped (identity, values, relationships). The gadget will say so when that's true.
- Not unlimited scope. It refuses pains too large for a one-week starter.

See `EVALUATE.md` for the scorecard.
