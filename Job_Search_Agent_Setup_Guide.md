# Setting Up Your Job Search Agent - Quick Start

No coding. About an hour of writing, plus a few minutes of clicking to connect tools.

## What you'll need before you start

- Access to Claude (claude.ai, Claude Code, or Cowork; any of them work).
- A place for the agent to search jobs (a job board connector, or you're fine with it using general web search).
- A spreadsheet (Google Sheets is the easy default). This is the agent's memory.
- Optional: email (so digests land in your inbox instead of only in the chat).

## Steps

**1. Make a project folder.**
Something like "Job Search Agent." Everything below lives here.

**2. Get the questionnaire and fill it out.**
Answer honestly, especially the "honest gaps" and "jobs you'd reject" sections. Those matter more than anything else in the document. "You decide" is a fine answer when you're not sure.

**3. Check what tools you actually have connected.**
This agent runs on MCP connectors, small plug-ins that let Claude actually talk to outside services instead of just describing what it would do. At minimum, check for: a job source (for example, an Indeed MCP), a spreadsheet (a Google Drive/Sheets MCP), and, if you want digests emailed to you, an email connector (a Gmail or Outlook MCP).

In Claude Desktop, these live under Settings, then Connectors (click your profile icon or the menu in the corner, then "Connectors"). That screen shows what's already connected and lets you browse and add more from the directory. Do this check before you answer the sourcing and output questions in the questionnaire; the agent can only use what's actually connected there, no matter what the manual tells it to do.

**4. Hand Claude the completed questionnaire.**
Paste in the generation prompt included at the bottom of the questionnaire. Claude will produce your operating manual.

**5. Read the manual it gives you back.**
Fix anything that doesn't sound like you, especially the scoring rubric, the hard rules, and the resume tailoring rules. This is the one step worth not rushing.

**6. Save everything into your project folder.**
The manual, your resume, and (if you split it out) your story bank.

**7. Set up your spreadsheet and connect it.**
Create a blank tracking sheet with the columns your manual expects, and make sure Claude can read and write to it.

**8. Run one test of each piece before trusting it.**
Ask for one digest and one tailored resume. Check that the format matches what you asked for and nothing sounds fabricated.

**9. Turn on the schedule, if you want it automatic.**
Ask Claude to schedule the digest for the cadence you specified (for example, Monday/Wednesday/Friday mornings).

**10. Check in every week for the first month.**
Skim what it surfaced, correct anything off, and update the manual. After the first month, monthly check-ins are usually enough.

That's it. Steps 1-6 are writing, 7 is a few clicks, 8-10 are just running it and watching.
