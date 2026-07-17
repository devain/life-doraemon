# build-your-own-gadget — evolutionary scorecard

| Test | Score | Reasoning |
|---|---|---|
| **Capability transfer** | Pass | The whole point is to teach the design move. Restated problem + latent need + smallest dissolve is a transferable pattern. After ~5 uses, the user can run the move on their own pains. |
| **Reach extension** | Pass | Gets non-developers to attempt tool-design who wouldn't otherwise. Output is usable artifacts, not theory. |
| **Teaching surface** | Pass | Each section names *why* — why this restating, why this dissolve, why this evolutionary frame. The reasoning is the lesson. |
| **Long-run effect** | Conditional | User must apply the pattern, not just collect tools. The README explicitly warns about this; the prompt refuses to deliver if the user is in tool-collection mode. |
| **Friction respect** | Pass | Removes the wasteful friction of "I don't know how to start." Preserves the productive friction of actually using the thing and iterating. |

**Score: 4 hard passes + 1 conditional.** Qualifies.

## The recursion

This gadget builds gadgets. Each gadget it builds should itself pass the evolutionary test. The prompt forces this — if the model can't honestly answer "what skill will the user gain?", the gadget is flagged as not-Life:Doraemon. The recursion is the integrity check.

## Failure mode to refuse

Tool-collection without practice. If the same user keeps requesting gadgets without using any of them, the catalog grows but the user doesn't. v0.2 idea: track "pain ids" the user has submitted; warn on repeat-pain without a follow-up signal.

## Sign-off

The meta-gadget is the highest-leverage entry in the catalog — every other gadget can come from this one. But it is also the most dangerous if mis-used (tool-collecting). Honor the warnings in the prompt.

Date: 2026-05-15
Version: 0.1
