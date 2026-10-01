# Custom Instructions -- career-ops

<!-- ============================================================
     THIS FILE IS YOURS. It will NEVER be auto-updated.

     Put your own house rules, custom workflows, and automations
     here -- anything you want the agent to ALWAYS do (or never do).

     This is for PROCEDURAL rules ("HOW I want things done").
     For WHO you are (archetypes, narrative, comp, negotiation),
     use modes/_profile.md instead. Keeping the two separate keeps
     each one readable.

     The agent reads this file alongside the system instructions;
     your rules here take precedence over the defaults, as long as
     they don't break the Data Contract (your files are never
     touched, and we never auto-submit an application for you).

     Because this is a user-layer file, anything you write here
     survives `node update-system.mjs`. Put customizations HERE,
     not in CLAUDE.md / modes/_shared.md / other system files --
     those get overwritten on update.
     ============================================================ -->

## House Rules

- Every `scan` run (including the recurring automated loop) must also check these sources that `scan.mjs`'s zero-token providers cannot reach, since they have no public Greenhouse/Lever/Ashby-style API:
  - **NATO bodies**: NCIA (NATO Communications and Information Agency, ncianato.referrals.selectminds.com / nato.taleo.net), NATO HQ (nato.int/recruitment vacancy PDFs), and NSPA (nspa.nato.int) — via WebSearch + WebFetch, looking for QA / Quality Assurance / Test Engineer / Test Automation / Software Test / Service Quality roles. Verify each hit against the institution's own listing before reporting it (these portals' search results are JS-rendered and search-engine snippets often surface expired postings).
  - **Belgium and Netherlands, company-by-company**: in addition to whatever VDAB/job-board hits `scan.mjs` turns up, run a targeted WebSearch pass for QA/Test Automation openings at well-known NL/BE tech employers (e.g. Adyen, Booking.com, Picnic, bol.com, Mollie, Deliverect, Proximus, Colruyt Group) and verify liveness on each company's own careers page/ATS before reporting a match.
- Apply the same ghost-posting verification discipline to these as to everything else: primary-source confirmation, not aggregator text; flag staffing/placement-agency postings (unnamed end client) as a distinct category, since I generally decline those in favor of direct employment.

## Custom Workflows

(none yet -- add yours above)

## Output Preferences

(none yet -- add yours above)

## Off-Limits

(none yet -- add yours above)
