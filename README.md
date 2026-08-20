# Job Search Agent

An autonomous job search pipeline built on Claude and MCP connectors. It sources roles on a schedule, screens and scores them against my own criteria, flags anything ambiguous back to me instead of deciding alone, and reports out. I built it after being laid off, to replace the hours I was spending manually re-checking the same job boards every day.

## The problem

Job searching is mostly repetitive triage: check the same handful of sources, filter out roles that were never going to work, and evaluate the ones that might. I was doing that by hand for hours a day, inconsistently, some days thorough, some days rushed, with no record of why I'd already passed on a role when it resurfaced under a new posting three weeks later.

This is what I built to take that over: a written rulebook that Claude follows on a fixed schedule, plus a handful of tool connections that let it actually search, track, and report instead of just describing what it would do.

## What it does

- Sources roles on a cadence I set
- Filters out anything that fails a hard rule (wrong geography, below my salary floor, a company I've excluded) before spending any real evaluation effort on it
- Scores everything that survives against a six-dimension rubric, first on cheap search snippets, then in full detail only for the finalists
- Flags anything ambiguous back to me instead of deciding alone: borderline salary, a company that already rejected me once, a role that's borderline on several dimensions at once
- Tailors my resume to a specific role on request: a short delta by default (new summary, reordered bullets and skills, a rationale), a full formatted document only when I ask for it
- Writes every result to a tracking spreadsheet and emails me a formatted digest
- Never submits an application. I do that myself

## Demo

[`Sample_Digest.html`](./Sample_Digest.html) is a full example of the output, built around a fictional search so it's safe to share. [`Sample_Operating_Manual.md`](./Sample_Operating_Manual.md) shows what the generated rulebook behind it looks like.

## How it works

Six stages: trigger, source, filter, score, escalate, record and notify. The two-stage scoring, the escalation model, and the company and pipeline state tracking are the parts worth understanding if you're adapting this yourself, all covered in [`Architecture.md`](./Architecture.md).

## Design decisions worth knowing about

- **Scoring is two-stage.** A cheap snippet pass first, full detail only for the finalists, to control cost.
- **Not everything is automated.** Applying, resolving an ambiguous call, and changing the underlying criteria all stay a human decision on purpose, not because they're hard to automate.
- **The rulebook is versioned.** Every change gets logged with a reason, so a decision I've already made doesn't quietly get re-asked a few weeks later.

## Tech stack

- Claude, running on a schedule
- MCP connectors for the job source, a spreadsheet (the tracker), and email (digest delivery)
- A single markdown file as the entire "program." No custom backend.

## Limitations

Sourcing quality varies day to day; some runs turn up a strong slate, some turn up almost nothing, and a thin digest is a legitimate output, not a bug. The system is only as good as the rubric written into the manual; it has no independent judgment beyond what's specified. And there's no automated apply step, on purpose, since that's the one action that's expensive to take back.

## Want to build your own?

This repo includes everything I used to build mine:

| File | What it's for |
|---|---|
| [`Job_Search_Agent_Questionnaire_Template.md`](./Job_Search_Agent_Questionnaire_Template.md) | Fill this out first. It's what turns into your own operating manual. |
| [`Job_Search_Agent_Setup_Guide.md`](./Job_Search_Agent_Setup_Guide.md) | The very-basic, step-by-step version of getting from a blank questionnaire to a running agent. |
| [`Sample_Operating_Manual.md`](./Sample_Operating_Manual.md) | A fictional example of what a completed questionnaire turns into. |
| [`Sample_Digest.html`](./Sample_Digest.html) | A fictional example of the actual output. |
| [`Architecture.md`](./Architecture.md) | How the system is designed, and why, for anyone adapting it. |
| [`LICENSE`](./LICENSE) | MIT. Copy it, adapt it, make it yours. |

Start with the Setup Guide.

## About this project

I'm Riley, a product manager. I built this to close the gap between product intuition and hands-on AI and agent-building fluency, while actually solving a problem I had. Happy to talk through any of it.
