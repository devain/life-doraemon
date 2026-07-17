# brief — evolutionary scorecard

The plan requires every gadget to pass the **evolutionary test** before it counts for the catalog. This is the design-time scorecard for `brief` v0.1.

## The five tests

| Test | Question | How `brief` answers it |
|---|---|---|
| **Capability transfer** | Does it leave a skill *in* the user, or take effort away from them? | The "Why these, not others" section teaches the filter pattern. The user sees what was cut and why. After 50 uses on different topics, the filtering logic becomes familiar — the user can run it themselves for known domains. **Pass (designed for).** |
| **Reach extension** | Does it expand what they can reach, or replace their own movement? | Reach-extending: primary sources are listed; the user must read them. The brief is a pointer, not a substitute. **Pass.** |
| **Teaching surface** | Does it teach as it serves, or hide what's happening? | Explicit teaching surface section. The prompt forces it. **Pass.** |
| **Long-run effect** | After 1000 uses, is the human stronger or weaker? | Stronger IF they use it as designed (read the sources, internalize the pattern). Weaker IF they treat the brief as the destination. The design pushes them right; the prompt warns against the failure mode; but the user has to honor it. **Conditional pass.** |
| **Friction respect** | Does it preserve the productive friction, removing only the wasteful kind? | Removes the wasteful friction of "where do I start?" Preserves the productive friction of "now read the actual sources." **Pass.** |

## Score

**4 hard passes + 1 conditional pass.** Qualifies for the catalog.

## Weakness to fix in v0.2

The conditional pass on "long-run effect" depends on the user not weaponizing the brief into a substitute for reading. Two ways to harden:

1. **Cap source-less reuse.** If the same topic is briefed twice in a week, the v0.2 could refuse and ask whether the sources from last time were actually read.
2. **Surface progress.** Track topics briefed; ask the user to mark which ones they followed up on. Visibility creates accountability with themselves, not me.

## Sign-off

This scorecard is what makes `brief` a catalog gadget, not just a prompt. Reviewing the test was the act that proved the gadget is in the right shape.

Date: 2026-05-15
Version: 0.1
