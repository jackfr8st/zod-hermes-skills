---
name: deadline-triage
description: Turn pasted job, internship, grant or course notices into a dated list of REQUIRED deadlines versus OPTIONAL events, with a follow-up plan. Text-only; never submits, registers or emails anything.
version: 1.0.0
license: MIT
compatibility: Hermes Agent v0.22.7 or later. Needs no tools, plugins, credentials or network access.
metadata:
  hermes:
    tags: [deadlines, applications, planning, students]
---

# Deadline triage

This skill is a set of instructions, not a tool: there is nothing to call. Read the notice the
user pasted and answer directly in the format below.

Always answer with exactly these four headings, in this order: `REQUIRED`, `OPTIONAL`,
`INFO`, `NOT DONE YET`. Put each dated item under one heading.

Use this skill when the user pastes one or more notices (job or internship postings, grant
calls, course announcements, recruiter emails) and asks what is due, what is optional, or
what to do next. Work only from the pasted text. Do not browse, call tools, or contact anyone.

## Procedure

1. **Find every dated item.** For each date or time in the text, note what it is and copy the
   exact wording that states it. Keep the time zone exactly as written. If no time zone is
   given, say "time zone not stated" instead of guessing.
2. **Classify each item.**
   - **REQUIRED**: something the user must deliver or do (submit, apply, upload, register by).
   - **OPTIONAL**: something the user may attend or use (info session, Q&A, office hours,
     networking event), or anything described as optional, recommended or encouraged.
   - **INFO**: dates that need no action (decision release, program start).
   If the wording is ambiguous, classify it as REQUIRED and say why.
3. **Name the source.** If the notice has an ID, title or sender, cite it next to each item.
4. **Check status claims.** Never state that something was submitted, registered or sent
   unless the pasted text says so. If the text says nothing was submitted, repeat that.
5. **Plan follow-ups.** For each REQUIRED item, propose one preparation step dated at least
   two days before the deadline (or "as soon as possible" if less than two days remain).
6. **Answer in this format:**

```
REQUIRED
- <what> — due <date, time, zone> — source: <id or title> — prep: <step and date>
OPTIONAL
- <what> — <date, time, zone> — source: <id or title>
INFO
- <what> — <date> — source: <id or title>
NOT DONE YET: <what the text says has not been submitted, or "status not stated">
```

Keep the answer short. Do not invent deliverables, dates, links or contact details. See
[references/example.md](references/example.md) for a worked example.
