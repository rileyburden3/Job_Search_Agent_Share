# Job Search Agent Setup Questionnaire

Fill this out, hand it to Claude, and ask it to build your agent operating manual. Answers can be short. "You decide" is a valid answer for anything you are unsure about.

Estimated time: 60 to 75 minutes.

---

## PART 1: WHO YOU ARE

**1.1 Basics**
- Name:
- Location (city, state):
- Email and phone:
- LinkedIn or portfolio URL:
- Current status (employed, laid off, actively looking, casually looking):

**1.2 Career arc**
List each role in reverse order: company, title, dates, one line on what you owned.

*Example: Acme Corp (2021 to 2025), Senior Analyst, owned forecasting models for a $400M business line.*

**1.3 Your top 5 differentiators**
What makes you stand out? Be specific. Not "strong communicator." More like "built a partner program from zero that brought 10 partners to market."

1.
2.
3.
4.
5.

**1.4 Your honest gaps**
This is the most important question in the questionnaire. The agent needs to know what you cannot credibly claim, or it will write resumes that get you screened out or embarrassed in interviews.

*Examples: no formal degree in the field, no hands on technical depth in X, most recent projects did not ship, limited experience in regulated industries.*

1.
2.
3.
4.

**1.5 Paste your current resume**
Paste the full text. This becomes the agent's source of truth for tailoring.

**1.6 Resume format rules**
The agent needs to know what it is allowed to change and what must stay fixed. Without this it will quietly restructure your resume every time it tailors it.

- Length limit (one page, two pages, no limit):
- Section order you want preserved (example: summary, core competencies, experience, earlier experience, education):
- Anything that must never move or change (example: contact block, education section, job titles and dates):
- Formatting constraints (example: plain text only, no tables or columns or graphics, since applicant tracking systems often fail to parse them):
- Do you want a single master resume that gets tailored each time, or several base versions for different role types:
- Do you have a specific visual template (fonts, colors, table-based layout) you want preserved exactly, or is content-only tailoring enough:

*Example answer: two pages maximum, section order fixed, titles and dates never change, plain text with no tables, one master version.*

---

## PART 2: WHAT YOU ARE LOOKING FOR

**2.1 Target titles, in order of preference**
1.
2.
3.

*Note any title translation issues. Example: "my current title is inflated relative to the market, so do not filter out roles one level down."*

**2.1b Adjacent titles**
Are there titles outside your primary track that your background genuinely maps to, even though the title itself doesn't match (example: your product management background also fits Strategy & Operations or Partner Ecosystem roles)? List them here as legitimate parallel targets, not fallbacks, and note any seniority floor that applies (example: "no entry-level, but title-level filtering otherwise doesn't matter, only scope and pay do").

1.
2.
3.

**2.2 Geography rules**
- Ideal (specific cities or neighborhoods):
- Acceptable with flexibility:
- Acceptable only if fully remote:
- Ask me before recommending:
- Never surface:
- How to handle a posting that's ambiguous about location (example: "Bay Area" or "hybrid" with no city or on-site frequency stated): hold it back for confirmation, or score it as if it were the most likely reading and only escalate once it's confirmed to be the bad case:

**2.3 Compensation**
- Base salary floor (hard number):
- Expected range for your level:
- How to handle roles slightly below floor (auto reject, or ask you first):
- How to handle roles with no salary posted at all (assume above floor, assume at floor, or stay neutral and say so explicitly):

**2.4 Industries**
- Open to all, or specific list:
- Any industry to exclude entirely:

**2.5 Company size**
- Open to all, or preference (startup, mid market, enterprise):
- Any concerns about equity heavy compensation at early stage companies:

**2.6 Companies to exclude, and how that should evolve**

A flat "never show me this company" list breaks down within a few weeks of real use. In practice you'll want at least three different kinds of exclusion, and they behave differently:

- **Paused**: temporary. You have an active application in review, or the company had layoffs and you don't want new reqs surfaced right now. You lift the pause yourself when ready.
- **Suppressed**: permanent. No resurfacing without you explicitly asking for that company by name again.
- **Ask before resurfacing**: you were rejected by this company once, under one req. A different req or team later is worth a look, but the agent should flag it and ask rather than deciding alone.

List what you know now, and mark the type:

| Company | Reason | Type (Paused / Suppressed / Ask before resurfacing) | Revisit condition |
|---------|--------|------------------------------------------------------|--------------------|
| | | | |
| | | | |

Also decide: if a company keeps clearing your score threshold but you keep passing on it anyway across several different reqs, should the agent flag that as a pattern worth discussing rather than treating each new req as unrelated?

Your answer:

**2.7 Work model preference, ranked**

This is about *how* you work, not *where* the office is (that was 2.2). Rank these from most to least desirable so the agent knows how to break ties between two otherwise equal roles. Copy the ones that apply and put them in your order, or write your own.

Common options:
- Fully remote, no office requirement
- Hybrid, 1 to 2 days per week on site, office close to home
- Hybrid, 3 days per week on site, office close to home
- Hybrid, occasional on site travel to an office that is far away
- Fully on site, office close to home
- Remote first, with optional office access nearby

Your ranking:
1.
2.
3.

Also note any hard limits. *Example: "anything above 2 days per week on site is a no, regardless of how good the role is."*

---

## PART 3: HOW THE AGENT SHOULD SCORE JOBS

**3.1 Scoring dimensions**
Most people use 5 or 6 dimensions. Here is a starting set. Adjust, rename, or replace as needed.

| Dimension | What it measures | Keep or change |
|-----------|------------------|----------------|
| Experience match | Do you meet 60 to 70 percent of stated requirements | |
| Title and seniority | Is the level right for you | |
| Geography and commute | Does the location work | |
| Compensation | Does the pay clear your floor | |
| Domain signal | Does the role value your specific background | |
| Recruiter attention | Would a recruiter spend more than 15 seconds on your resume for this | |

Add any dimension specific to your situation (visa sponsorship, security clearance, travel percentage, industry regulation).

If you added an adjacent-titles tier in 2.1b: should scoring calibrate differently for those titles (example: don't penalize the Title/Seniority dimension just because the title doesn't literally match your primary track, if the scope and level are equivalent)?

Your answer:

**3.2 Scoring scale**
- 1 to 10 per dimension, or a single composite score:
- Threshold for GO:
- Threshold for CONDITIONAL:
- Threshold for NO:

*Common default: score each dimension 1 to 10, average them. 8.0 and up is GO, 6.0 to 7.9 is CONDITIONAL, below 6.0 is NO.*

**3.3 Auto flag rule**
Should a single very low dimension score override a good average? Example: "if any dimension scores 3 or below, flag it for my review regardless of average."

**3.4 Scoring overrides and caps**

Averaging dimensions can hide one disqualifying trait behind a strong overall number. Decide what should cap a specific dimension regardless of how well the rest of the role reads. This is different from 3.3: 3.3 is about flagging you for review, this is about the score itself refusing to go above a ceiling.

Common override patterns to consider:
- A hard technical skill listed as a must-have that you don't have (a specific language, tool, or certification): caps Experience Match low even if everything else fits.
- A domain you have zero background in (a specific regulated industry, a specific technical subfield): caps Experience Match, as a separate rule from the one above.
- A role-type-specific penalty for a category you're targeting that has a known failure mode (example: if you're open to Product Marketing roles alongside Product Management, cap domain fit lower by default when the role is really content or campaign execution rather than positioning and launch strategy).

List your own override rules, and which dimension each one caps:

1.
2.
3.

**3.5 Gray-zone rule: what happens with a borderline CONDITIONAL**

A CONDITIONAL score is not automatically apply-worthy. Decide the rule for the space between "clearly no" and "clearly yes," or the agent will end up recommending you apply to everything that clears the minimum bar.

- Where's the line between "apply by default" and "don't apply unless you have a specific reason"? *Example: 8.0+ = GO, apply. 7.0 to 7.9 = CONDITIONAL, apply by default. 6.0 to 6.9 = CONDITIONAL, default to Not Pursuing unless you log a specific reason to stretch.*
- Should applying below that line ever require you to write down why, so it's a deliberate choice rather than a drift?

Your answer:
- Apply-by-default line:
- Requires a logged reason below that line: Yes / No

Also decide: should the agent ever let volume against your weekly cap (Part 6.5) substitute for fit? *Recommended default: no. A week with fewer, stronger applications beats a week padded with below-threshold ones to hit a number. If that's your instinct too, say so explicitly and ask the agent to flag it if it notices this happening more than once or twice in a rolling two-week window.*

Your answer:

---

## PART 4: CALIBRATION EXAMPLES

This section teaches the agent your judgment. It is worth more than any amount of criteria writing.

**4.1 Three jobs you would love**
For each: company, title, and two sentences on why it is a strong fit.

1.
2.
3.

**4.2 Three jobs you would reject**
For each: company, title, and two sentences on why you would pass. Pick ones that look good on paper but are actually wrong for you.

1.
2.
3.

**4.3 Green flags**
Patterns that make you want to apply immediately.

**4.4 Yellow flags**
Things you will tolerate but want called out.

**4.5 Red flags**
Automatic disqualifiers.

---

## PART 5: YOUR VOICE

**5.1 Resume bullet style**
Paste two bullets you wrote yourself that you are proud of. The agent will pattern match on these.

Good example:

Bad example (write one in the style you want the agent to avoid, usually corporate buzzword soup):

**5.2 Words and phrases to never use**
*Examples: leverage, synergy, passionate about, thrilled to apply, cutting edge.*

**5.3 Your story bank**
List 6 to 10 situations you can draw on for interviews. One line each: theme, situation, outcome.

| Theme | Situation | Outcome |
|-------|-----------|---------|
| Influence without authority | | |
| Disagreed with leadership | | |
| Decision with incomplete information | | |
| Changing requirements | | |
| Missed a deadline | | |
| End to end ownership | | |

---

## PART 6: YOUR CURRENT PIPELINE

**6.1 Active opportunities**
Company, stage, any relevant context.

**6.2 Closed pipeline**

Keep a running record of what's closed and why, separate from active. This is the single thing that stops the agent from re-suggesting a company you already got a no from under a different requisition. An active-only list forgets history the moment something closes.

For each: company, what happened, when, and whether it should ever come back.

| Company | Outcome (rejected / withdrew / went stale / paused) | Date | Resurface rule (never / ask me first / automatically if X) |
|---------|-------------------------------------------------------|------|----------------------------------------------------------------|
| | | | |

**6.3 Patterns you have noticed**
Where are you getting stuck? Examples: not getting past resume screen, stalling after first interview, getting to final rounds and losing.

**6.4 Your hypothesis on why**
Best guess at the root cause. The agent will use this to focus its help.

**6.5 Weekly application cap**
How many applications per week is realistic for you to do well? Most people should stay under 10.

---

## PART 7: HOW THE AGENT SHOULD OPERATE

**7.1 Job sources**

Your agent can only pull from sources it is actually connected to. Check what connectors (MCPs) you have available in your Claude settings before answering.

Commonly available as direct connectors:
- Indeed
- ZipRecruiter

Reachable through general web search, but not as a direct connector:
- Company career pages
- Applicant tracking systems that host public job boards (Greenhouse, Lever, Ashby, Workday)
- Niche or industry specific boards

Not available and should not be attempted:
- LinkedIn. There is no public connector, and scraping it violates their terms of service. Treat LinkedIn as a manual source: browse it yourself once or twice a week and paste promising job URLs into the agent for scoring.

Your answers:
- Connectors you have enabled:
- Primary source (the one the agent should always try first):
- Secondary sources (only used when the primary comes up short):
- Sources to avoid entirely:
- Will you feed in manual URLs, and how often:
- If you name specific "priority companies" whose career pages should be checked every run regardless of what the primary source returns: should the agent verify a posting is still live before scoring it, or is scoring a possibly-stale posting an acceptable risk? *A live-check costs an extra step per company but avoids wasting a full scoring pass on a pulled posting.*

**7.2 Cadence**
- How often should the digest run (daily, every other day, three times a week):
- What days:
- What time:

*Three times a week is a good default. Daily burns tokens without surfacing much new inventory.*

**7.3 Digest size and format**

Decide the shape of the output now. If you do not, the format will drift from run to run and you will not be able to compare jobs at a glance or scan the digest quickly on your phone.

- How many jobs per digest (3, 5, 7, 10):
- Summary table plus per job detail, or detail only:
- Which fields belong in the summary table (example: rank, company, role, location, score, recommendation):
- Which fields belong in each detail block (see the sample below and cut or add as you like):
- Anything you want at the top of every digest (a one line headline, a count of how many were reviewed and filtered out):
- Anything you want at the bottom (open questions for you, escalations that need a decision):

Sample detail block. Mark it up rather than starting from scratch.

```
DETAIL: JOB #1, [Company], [Role]
Link:
Location and work model:
Posted date:
Compensation (posted or estimated, say which):

Dimension scores:
  [Dimension 1]: X, one line reason
  [Dimension 2]: X, one line reason
  [continue for each dimension]
  AVERAGE: X.X, resulting in GO / CONDITIONAL / NO

Top 3 reasons for this recommendation:
  1.
  2.
  3.

Angle to lead with if I apply:
  [one specific recommendation, not generic advice]

Gaps to be aware of before applying:
  [honest assessment, or "none"]
```

If you are getting the digest by email, note any formatting preference for that specifically. Plain text survives every email client and is easy to scan on a phone. Heavy tables often break on mobile.

**7.4 Where output goes**

Two separate decisions here: where you *read* the digest, and where the data *lives* over time.

Delivery options (how you read it):
- In the chat window only. Simplest, no setup, but you have to open the app to see it.
- Emailed to yourself. Best if the digest runs on a schedule, since you check email more reliably than you open a chat app. Requires a Gmail or Outlook connector.

  Note: depending on how your email connector is set up, Claude may not have permission to actually send mail on your behalf, only to draft it. If that's the case, your digest will sit in your Drafts folder instead of landing in your inbox. Check your Drafts folder the first few times a scheduled digest is supposed to arrive, so you're not left wondering why nothing showed up.
- Written to a document in cloud storage. Good if you want a running archive. Requires a Google Drive or similar connector.
- Some combination. Common pattern: emailed to you, and every job also written to a tracking sheet.

Storage options (where the data lives):
- A tracking spreadsheet is strongly recommended (Google Sheets is a common, easy choice if you already have a Drive connector). It is the agent's memory across sessions and the only way it can avoid showing you the same job twice or calculate your success metrics later.
- Typical columns: date added, company, role, location, source, link, fit score, recommendation, status, date applied, notes.
- The status column is yours to fill in. Suggested values: need to review, need to apply, applied, interviewing, rejected, not pursuing.

Your answers:
- How the digest reaches you:
- Tracking spreadsheet: yes or no:
- Where it lives and what it is called:
- Any other output destination (a folder for tailored resumes, for example):
- If Status is set to Applied on any row, should Date Applied be mandatory at that point, so application-rate metrics stay accurate:

**7.5 Escalation rules**
When should the agent stop and ask you instead of deciding? List specific scenarios.

*Examples: role is in a borderline location, pay is slightly under floor, company already rejected you, more than the digest cap cleared the bar, 3 or more dimensions all landed in a mediocre middle range at once (which usually means "nothing is disqualifying but nothing is compelling either" and is worth a human read).*

**7.6 Closing out escalations**

Once you answer an escalation question, that answer should stick. Decide: when you resolve one (you confirm a specific city is fine, or a specific salary band is acceptable), should the agent record that as a standing decision and stop asking about it going forward, or ask fresh every time it comes up?

*Recommended: record it as resolved and close the flag; only reopen if you say so. This only works if the manual has somewhere to log resolved decisions, see Part 12. Otherwise the same question quietly gets re-asked every week, and after enough of that you'll stop reading the escalation section at all.*

Your answer:

**7.7 Recruiter outreach exception**

If a recruiter proactively reaches out about a role that would otherwise score NO, is that different from you overriding the filters yourself? Most people say yes. Proactive outside interest is a signal the scoring rubric can't see on its own.

Your answer:
- Allow recruiter-initiated outreach to bypass scoring: Yes / No
- If yes, any cap on how often, so the exception doesn't quietly become the rule (example: no more than one per week):

**7.8 Hard rules**
Things the agent must never do.

*Examples: never claim skills you do not have, never auto submit applications, never surface excluded companies, never invent metrics.*

---

## PART 8: TOKEN EFFICIENCY

Agents that search the web and read full job descriptions consume tokens quickly. Decide these up front.

**8.1 Source priority**
Should the agent try one primary source first and only search more broadly if that comes up short? (Recommended: yes.)

**8.2 Two stage scoring**
Should the agent score on search result snippets first, then fetch full job descriptions only for finalists? (Recommended: yes. Set a finalist count, usually 8 to 12.)

**8.3 Output verbosity**
For tailored resumes, do you want the full document every time, or only the parts that changed? (Recommended: only the parts that changed, with full output available on request.)

**8.4 Optional extras**
Which nice to have features should run only weekly rather than every digest? Examples: news monitoring on companies in your pipeline, market trend summaries.

**8.5 Run limits and self-reporting**

This runs on a metered subscription, often on an unattended schedule. Decide a hard stop for a single run, and what the agent owes you afterward.

- Max tool calls or steps before the agent should stop mid-task and report progress instead of continuing (a reasonable starting point is 25 to 35 for a sourcing-heavy run):
- Should the agent report its own resource usage at the end of every run, approximate tool call count, and a rough light / medium / heavy read on context consumption? *Recommended: yes, briefly. It's the only way you'll notice sourcing quality degrading, or a particular day's run running unusually expensive, before it becomes a pattern.*
- What should trigger a note to you outside the normal digest (example: a single run took more tool calls than the cap, a channel you rely on stopped returning useful results, you're about to burn an unusual amount of your window on one task type):

---

## PART 9: SUCCESS METRICS

Pick 4 or 5 metrics you will actually look at. Set a target and a corrective action for each.

| Metric | Your target | What to do if off target |
|--------|-------------|--------------------------|
| Application rate (applied divided by surfaced) | | |
| Application to first conversation rate | | |
| First interview to second interview rate | | |
| Time spent reviewing each digest | | |
| Percentage of digest that matches your green flags | | |

---

## PART 10: REVIEW CADENCE

**10.1 Weekly retro**
- What day and time:
- What should it cover:

**10.2 Weekly judgment check**
Set aside 5 minutes before the retro to spot check the agent's calls. For each job it surfaced, ask: did it belong in the digest, was the score close to what you would have given, were the stated reasons the real reasons.

- Your passing threshold (example: 12 out of 15 feel right):

**10.3 Monthly structural review**
- What day:
- Focus: patterns in what the agent got wrong, systematic scoring biases, whether criteria need to widen or narrow.

**10.4 Who evaluates the agent**
The agent reports data. You judge quality. The agent cannot tell you whether its own judgment is good, so plan to check its work yourself.

---

## PART 11: FILE STRUCTURE

You do not need one giant file. Splitting content that changes at different rates keeps the operating manual readable and stops the agent from re-reading a long document it does not need for the task at hand.

Recommended structure for a project folder:

```
Job Search Agent/
  operating-manual.md      the rules: criteria, scoring, workflows, hard rules, changelog
  resume-master.md         your baseline resume, the source of truth
  story-bank.md            your situations for interview prep
  tracker link or file     the spreadsheet, or a note pointing to it
  outputs/                 tailored resumes the agent produces
```

Why split these three:

- **The operating manual** changes weekly at first. Keep it tight so you will actually revise it.
- **The resume** changes rarely but is long. Separating it means the agent reads it only when tailoring, not on every digest run.
- **The story bank** is referenced only for interview prep. Same logic.

If you would rather keep everything in one file, that works too. Just expect it to run long, and expect to pay for that length in tokens on every single task.

**A note on formal Skills.** Claude supports a packaged format called a Skill, which is a folder containing a SKILL.md file plus supporting resources, and which the model loads automatically when a task matches its description. That is a different thing from the plain markdown files above, and for a personal job search agent it is usually more machinery than the job requires. Consider building one only if you want the same behavior to trigger automatically across many different projects, or you want to hand the whole setup to someone else as a single installable package. For one person running one search in one project folder, plain markdown files plus project instructions are enough.

Your answer:
- One file or split into several:
- If split, which files:

---

## PART 12: KEEPING THE MANUAL ALIVE

Everything above produces a manual that's accurate on day one. This part is about what keeps it accurate in month three, once companies have moved between paused and active, escalations have been answered, and criteria have drifted from where you started. Skipping this part is the single most common reason a well-built manual quietly goes stale.

**12.1 Version history**

Ask Claude to add a dated changelog table at the bottom of the operating manual, and to *append* an entry rather than silently overwrite whenever a rule changes. Each entry should say what changed and why, ideally tied to the date you confirmed it. This is what lets a resolved escalation (Part 7.6) stay resolved instead of quietly reopening a few weeks later, and it's the record the monthly review (Part 10.3) actually works from: "did I mean to change this, or did it drift."

A simple table is enough: version, date, what changed, one line why.

**12.2 Who's allowed to change what**

Decide which changes the agent can make on its own versus which always require your review before they land in the manual.

*Recommended default: the agent can update things you've told it directly (closing an escalation you resolved, updating a Status field, pausing or resuming a company at your instruction) without asking again. Anything that changes targeting criteria, scoring thresholds, or your resume's source of truth gets proposed at the weekly or monthly retro and you approve it before it's written.*

Your answer:
- Agent can update without asking:
- Agent must propose and wait for approval:

**12.3 Manual vs. tracker as source of truth**

If both a tracking spreadsheet and the operating manual record pipeline or company status, decide which one wins when they disagree. This happens more often than it sounds like it should, once the manual is a few months old and has been updated in a different session than the tracker.

Your answer:

---

## HOW TO USE YOUR COMPLETED QUESTIONNAIRE

1. Fill this out honestly, especially Part 1.4 (gaps) and Part 4 (calibration examples).
2. Hand it to Claude with this prompt:

```
Here is my completed job search agent questionnaire. Build me a complete
agent operating manual in markdown.

STRUCTURE
Numbered sections covering: who I am, targeting criteria, scoring
framework, my resume, resume tailoring rules, green and red flags,
current pipeline (active and closed), agent workflow, hard rules,
token efficiency rules, success metrics, evaluation cadence, and a
version history changelog.

REQUIRED TEMPLATES
Include three explicit templates, written out in full so the agent can
follow them exactly rather than improvising:

1. Digest output format: summary table columns and per-job detail
   block, matching Part 7.3.
2. Resume tailoring output spec: exactly which parts of my resume the
   agent outputs when tailoring, what it must never change, and the
   format constraints from Part 1.6.
3. Company and pipeline state-tracking convention: how paused,
   suppressed, ask-before-resurfacing, and closed-pipeline entries get
   recorded and updated (Parts 2.6 and 6.2), including how resolved
   escalations from Part 7.6 get logged so they don't get re-asked.

ALSO BUILD IN
- Scoring overrides and caps (Part 3.4)
- The gray-zone apply rule (Part 3.5)
- The recruiter outreach exception (Part 7.7)
- Run limits and self-reporting behavior (Part 8.5)
- A version history table at the bottom (Part 12.1), starting with a
  single entry marking this as the initial version

FILES
Split the output into separate files if I asked for that in Part 11.

TONE
Be specific and directive. Write it as instructions to an agent, not as
a summary of my answers. Where my answers were vague, make a reasonable
choice and flag it so I can correct it.
```

3. Read the output critically. Fix anything that does not sound like you.
4. Save it in a project folder your agent can read.
5. Test all three templates before you rely on them. Run one digest, tailor one resume, and pause one company then confirm the agent actually stops surfacing it. Formatting and logic problems are much cheaper to find now than in week three.
6. Update it weekly for the first month, then monthly, and check that updates are landing as new changelog entries, not silent rewrites.

The quality of your agent is the quality of this document. Revise it often.
