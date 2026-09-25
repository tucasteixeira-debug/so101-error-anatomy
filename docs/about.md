# About This Project

## The objective

Characterize and improve the placement repeatability of the SO-101 6-DOF
arm under a learned manipulation policy — measured independently of the
arm's own sensors — and identify whether the dominant source of error is
mechanical (backlash/compliance), control (servo tuning), or the learned
policy itself. Apply one targeted intervention and quantify the
improvement.

## Why this project

Physical AI — robots that combine perception, learning, and real-world
action — is what pulls me toward this space in the first place. It's
genuinely fast-moving right now: real commercial deployments already
exist, not just demos — Ambi Robotics and Pickle Robot announced the
first fully commercial truck-unloading-to-palletizing integration in
mid-2026, Agility Robotics' Digit runs in live Amazon warehouses, and
Boston Dynamics' Atlas is deployed at Hyundai. Humanoid platforms are
moving from lab demonstrations toward real pilots too — Figure AI's
robots have been tested on BMW's factory floor — though it's an honest,
mixed picture rather than a clean success story: that same pilot
reportedly ran at a fraction of human speed at first and needed a
hardware redesign along the way. Market-size projections for the space
vary by several times over depending which analyst you ask, which says
more about how unsettled the space still is than about its actual size.

Separately from the market picture, there's a specific, concrete gap
this project fills: the individual pieces it combines already exist on
their own — servo-level backlash characterization, ISO 9283-style
repeatability methodology, and a coarse benchmark of learned policies on
this exact hardware (which found execution instability, not perception,
is the dominant failure mode) — but nobody has yet combined them into
one quantified error budget for this platform. That's a real, specific,
citable hole, not a market claim.

I want to build genuine ability to work in this space and with this
technology — not stake out a specific lane within it yet, just get
real, hands-on capability and understanding.

## What I'm building toward

This project is deliberately structured to force real skills in, by
necessity, rather than studying them in isolation beforehand:

- **Full-stack technical maturity** — electronics, Linux, embedded
  systems, CAD, and control theory, each pulled in exactly when the
  build genuinely needs it
- **Conceptual fluency across the stack** — computer architecture,
  communication protocols, operating systems and the kernel, electronics,
  and embedded control systems — not just the high-level robotics/ML
  layer sitting on top of them
- **A mature, deliberate AI-assisted workflow** — using agents and
  Claude Code for real automation (build-log generation, recurring
  tasks), not ad hoc prompting
- **Real design judgment** — making and defending actual engineering
  decisions (measurement-rig design, the eventual intervention, task
  geometry) under real constraints, not following a prescribed path
- **An honest, dated build log** — this repo itself, written as the
  project happens rather than curated afterward
- **A genuine springboard** — a rigorous, portfolio-grade result
  relevant to physical-AI work, and a plausible foundation for further
  graduate research

## Where I'm starting from

Going in, my conceptual understanding across almost all of these areas
is close to zero — not just hands-on skill, but the underlying concepts
themselves: AI and machine learning, computer architecture, operating
systems, and most of Linux. I have some real prior exposure to embedded
control systems and electronics from earlier coursework, but it's
limited, not a strong foundation to build the rest from. The gap between
that starting point and what full-stack physical-AI work actually
demands is the real subject of this log, not something to smooth over.

## How I'm approaching it

One integrated build, not a series of separate exercises — every area
above gets pulled in only once the project genuinely needs it, learned
by doing rather than pre-studied. The measure of success isn't a flashy
end result; it's whether the engineering underneath it — the debugging,
the design choices, the honest dead ends — actually holds up.
