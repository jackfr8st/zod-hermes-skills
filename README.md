# zod-hermes-skills

A public [Hermes Agent](https://github.com/NousResearch/hermes-agent) skill tap created for CSCI 599 Assignment 3 (USC, Fall 2026) as part of the Zod assistant project.

## Skills

| Skill | Version | What it does |
| --- | --- | --- |
| [`deadline-triage`](skills/deadline-triage/SKILL.md) | 1.0.0 | Turns pasted job, internship, grant or course notices into REQUIRED deadlines vs OPTIONAL events, with a dated follow-up plan. Text-only: no tools, credentials or network. |

## Install on Hermes

```
hermes skills tap add <owner>/zod-hermes-skills
hermes skills install <owner>/zod-hermes-skills/deadline-triage
```

Then ask, for example: `Use the deadline-triage skill on this notice: ...`

All examples use fictional data. The skill never submits, registers or sends anything.
