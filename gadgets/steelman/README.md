# steelman

A steel-builder, not a sympathizer or a debater.

## The problem it dissolves

> Peace (one slice: the strawman trap).

Conflict escalates when each side argues against the weakest version of the other's view. The strongest version is usually invisible — not because no one holds it, but because most people only encounter the bad-faith summary. This gadget makes the strong version cheap.

## How to invoke

Two inputs:

| Input | Example |
|---|---|
| **View** | A view you find wrong / objectionable, in the form you encountered it (a tweet, a quote, a thread) |
| **My objection** *(optional)* | Why you think it's wrong (sharpens the steelman against your specific objection) |

Output:
- **The view at its strongest** — first-person upgrade of the position
- **The strongest case for it** — real evidence and reasoning
- **The legitimate values it serves** — what's good in the motivation
- **Genuine weaknesses** — honest weaknesses that survive the steelmanning
- **What you'd have to learn or accept** to find it compelling

## How to run

**Paste path:** open `prompt.md`, copy below the `---`, fill `{{VIEW}}` and `{{MY_OBJECTION}}`, paste into any Claude session.

**CLI path:** `.\steelman.ps1 -View "..." -MyObjection "..."` (needs `ANTHROPIC_API_KEY`).

## Evolutionary frame

- *Teaching surface*: the structure itself teaches steelmanning — first-person voice, values-naming, honest weaknesses
- *Capability transfer*: after enough uses, user pre-empts demonization and asks "what's the steelman?" before reacting
- *Failure mode*: confusing steelman with endorsement. The "genuine weaknesses" section keeps this honest.

## What it is NOT

- Not validation. Steelman is not "you're right." It's "this is the strongest version of what you might be missing."
- Not capitulation. The user keeps their own view; the gadget supplies a stronger opponent.
- Not for views that explicitly advocate harm against specific groups — the prompt declines those.

See `EVALUATE.md` for the scorecard.
