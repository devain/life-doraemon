# brief

A focusing lens, not an encyclopedia.

## The problem it dissolves

> Not enough time to know things AI don't know.

The need is *not* to know everything. It's to know **what's relevant to you right now, calibrated to what you already know, in the time you have.** AI as smart filter.

## How to invoke

You give it three things:

| Input | Example |
|---|---|
| **Topic** | "quantum computing" |
| **Minutes** | 15 |
| **Context** | "software engineer, never studied physics, building a side project that might benefit from quantum-inspired classical algorithms" |

You get back:

- **What you need to know** — 3-7 bullets, most relevant first
- **Why these, not others** — reasoning shown (this is the teaching surface)
- **Primary sources** — 2-5 things to read directly (no summaries; *you* integrate)
- **What I might be wrong about** — known weak spots, confidence calibration

## How to actually run it

**Option A — paste into any Claude session.** Open `prompt.md`, fill in your topic / minutes / context, paste. Free, instant, works in claude.ai or Claude Code or any tool that talks to Claude.

**Option B — PowerShell CLI.** Requires `ANTHROPIC_API_KEY` environment variable. Costs cents per call.

```powershell
.\brief.ps1 -Topic "quantum computing" -Minutes 15 -Context "software engineer, never studied physics"
```

or interactive:

```powershell
.\brief.ps1
```

## Evolutionary frame (what it must do to count)

- **Teaching surface**: shows its filtering reasoning, not just the answer
- **Capability transfer**: surfaces primary sources next to synthesis; user does the integration
- **Long-run effect**: after ~50 uses, user has internalized the filter pattern and can run it for familiar domains without the gadget

See `EVALUATE.md` for the test scorecard.

## What it is NOT

- Not an encyclopedia. It cuts ruthlessly.
- Not a summary tool. Summaries replace reading; this *prepares* reading.
- Not for entertainment learning. It's for time-constrained orientation.
- Not authoritative. It's a starting map. Use the sources.

## Failure mode to refuse

If the user starts treating the brief as the *end* rather than the *beginning*, the gadget has become a crutch. The prompt is designed to push against this — sources are surfaced, weak spots flagged, length kept short — but the design only works if the user honors it.

## Status

v0.1 — first run. Built 2026-05-15.
