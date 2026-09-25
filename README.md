# SO-101: Error Anatomy

Where does a learned robot policy's placement error actually come from?

This project breaks the placement error of the SO-101 6-DOF arm (Feetech STS3215 servos, Hugging Face LeRobot) into three contributions:
- **mechanical**: backlash and compliance
- **control**: servo tuning
- **policy**: the learned model itself

It uses ground-truth measurements taken independently of the arm's own sensors. Once the dominant source is known, one targeted intervention is applied and its effect quantified.

> **Status (2026-09):** hardware bring-up. The follower arm's servos are configured; leader arm setup and physical assembly are next. No measurement data yet.

## Navigating this repo

| Where | What you'll find |
|---|---|
| [`PROGRESS.md`](PROGRESS.md) | The dated build log. Start here to see what has actually been done |
| [`docs/`](docs/) | Background and objectives, plus methodology and results write-ups later |
| [`hardware/`](hardware/) | The physical platform: parts, bring-up status, and the measurement rig once it's designed |
| [`src/`](src/) | Code written for this project (measurement, analysis, experiment scripts) |
| [`experiments/`](experiments/) | One folder per experimental condition, each with its protocol, results and analysis |

Every folder has its own README explaining what goes in it and what state it's in.

## Suggested reading order

1. [`docs/about.md`](docs/about.md): why this project exists and what it's aiming for
2. [`PROGRESS.md`](PROGRESS.md): what has happened so far, newest first
3. Any folder README, depending on what interests you

## The approach, briefly

The same task is measured under progressively more complex conditions:

1. **Scripted motion** (no learning), which gives the raw mechanical + control repeatability
2. **A bench-level servo backlash test**, which isolates the mechanical share
3. **A trained policy**, which adds the policy's own variance on top

If these error sources are roughly independent, their variances add. Each contribution can then be estimated by subtraction. That independence is an assumption to check against the data, not something to take for granted.

## How this log is written

Build-log entries are drafted from private working notes with an AI-assisted workflow: Claude Code and a custom documentation skill. Each entry is reviewed and approved by hand before it is committed.
