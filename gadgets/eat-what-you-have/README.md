# eat-what-you-have

A kitchen lens, not a recipe encyclopedia.

## The problem it dissolves

> Food for everyone (household-scale slice).

The world wastes roughly a third of household food. Most waste happens because no one looks at what's already there before deciding what to cook. This gadget makes "look first" cheap.

## How to invoke

Three inputs:

| Input | Example |
|---|---|
| **Items** | "half cabbage, two eggs, leftover rice, a wilting tomato, onions, soy sauce, sesame oil" |
| **Constraints** | "vegetarian, ~20 min, 2 people" |
| **Mood** | "something warm" *(optional; leave blank if generic is fine)* |

Output:
- **Make this now** — one concrete meal you can cook from what's there
- **What's about to expire (act first)** — the items most likely going bad
- **Alternative** — backup meal using different items
- **What I'd add** — ≤3 grocery items, only if it really helps
- **What I might be wrong about** — calibration

## How to run

**Paste path:** open `prompt.md`, copy below the `---`, fill `{{ITEMS}}`/`{{CONSTRAINTS}}`/`{{MOOD}}`, paste into any Claude session.

**CLI path:** `.\eat-what-you-have.ps1 -Items "..." -Constraints "..." -Mood "..."` (needs `ANTHROPIC_API_KEY`).

## Evolutionary frame

- *Teaching surface*: reasoning shown — why this meal, what's expiring, what was skipped
- *Capability transfer*: user learns to *look* at the kitchen before planning. After 50 uses, the look becomes automatic.
- *Failure mode*: padding the meal with items they don't have. The prompt forbids this.

## What it is NOT

- Not a recipe app. It works only with what you list.
- Not a diet planner. It plans one meal from one set of ingredients.
- Not a substitute for actually opening the fridge.

See `EVALUATE.md` for the scorecard.
