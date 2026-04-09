# linkedin-outreach

A Claude skill for writing LinkedIn connection request messages and follow-up messages — built for job seekers reaching out to recruiters and HR contacts.

## What it does

Generates 2–3 message options for three scenarios:

- **Scenario A — Role-triggered**: You found a specific job and want to connect with the recruiter handling it
- **Scenario B — Exploratory**: You spotted someone relevant in your space and want to connect proactively
- **Follow-up**: They accepted your connection — what to say next (calibrated to whether they responded)

## Core principles

- A connection request is not a cover letter. It's a professional greeting.
- Avoids self-sell language ("strong fit", "matched my background well")
- Calibrates ask level to relationship stage — no CV/chat push before they've engaged
- Outputs multiple options with character counts (LinkedIn's 300-char limit)

## Install

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/sheltonyou/linkedin-outreach.git ~/.claude/skills/linkedin-outreach
```

Or install the `.skill` file directly via Cowork.

## Usage

Trigger phrases: "help me write a LinkedIn message to this recruiter", "I want to add this person on LinkedIn", "they accepted my connection, what do I say", 加猎头, LinkedIn跟进, 打招呼

## Built with

- [skill-creator](https://github.com/anthropics/skill-creator) — Claude Code skill framework
- Calibrated against 31 real LinkedIn connection requests and follow-up messages
- Iterated with human feedback across 3 eval scenarios
