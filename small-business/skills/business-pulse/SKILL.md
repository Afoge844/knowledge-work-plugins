---
name: business-pulse
description: >
  TEA-customized business pulse. Produces a one-page cross-functional snapshot
  for Art — content pipeline status (Notion), week-ahead commitments (Google
  Calendar), community health signals (Skool data if available), urgent email
  flags (Gmail), meeting/call follow-ups (Fireflies), and the single most
  important thing to act on today. Degrades gracefully — one connector gives
  a partial pulse; the full stack gives the full picture. Trigger when Art
  asks how the business is doing, wants a snapshot, a weekly summary, or says
  anything like "catch me up" or "what am I missing."
---

# TEA Business Pulse

One prompt, one page. Pull live data from every connected tool, synthesize into a single scannable brief, surface the one most important thing to act on today.

## Step 1 — Pull Data in Parallel

Dispatch all connector calls simultaneously. Do not pull serially.

**Notion** — pull:
- Content queue: items marked "ready to record", "ready to publish", or "overdue"
- Active workstreams: status of top 3 projects
- Course module tracker: current module, blockers, next step
- Any items flagged "urgent" or "this week"

**Google Calendar** — pull:
- All events today and next 7 days
- Any Saturday blocks (batch day — flag if unprotected)
- Deadlines, launch dates, or publishing commitments

**Gmail** — pull:
- Threads flagged urgent or containing "subscriber", "complaint", "cancel", "refund", "question"
- Any partnership or collaboration emails awaiting reply

**Fireflies** — pull:
- Any meeting transcripts from the past 7 days
- Action items or follow-ups flagged in transcripts

**Google Drive** — pull:
- Any files modified in the past 48 hours (signals active work)
- Anything in "ready to review" or "needs approval" folders

**Rainmaker/GHL** (if connected) — pull:
- New leads or subscribers in the past 7 days
- Funnel stage counts
- Any automations that failed or need attention

If a connector errors or returns no data, log it internally and move on. Never block the pulse on a single bad integration.

---

## Step 2 — Compute TEA Metrics

Assign 🟢/🟡/🔴 to each section. Mark "n/a" with a note if a source returned nothing.

**Content Pipeline Health:**
- 🟢 3+ items ready to produce or publish
- 🟡 1–2 items ready, nothing in queue after
- 🔴 Empty queue — no content ready for Saturday batch

**Saturday Batch Day:**
- 🟢 Saturday is blocked on Calendar with production time
- 🟡 Saturday has partial blocks or competing appointments
- 🔴 Saturday has no blocks — batch day is unprotected

**Community Pulse (if Skool/GHL data available):**
- Track: new member count WoW, engagement signals, any complaints or cancellations

**Course Progress:**
- Track: current module status vs. launch timeline

---

## Step 3 — Flag Risks Proactively

Every risk must name something specific with a next step. "Content queue is low" is useless. "No newsletter essay drafted for this Saturday — batch day is 3 days out" is actionable.

Scan for:
- Content queue empty or < 2 items ready
- Saturday batch day unblocked on Calendar
- Gmail threads with "cancel", "refund", or "complaint" unanswered > 48 hours
- Fireflies action items from past calls that haven't been acted on
- Course module in same status as last week (no progress)
- Substack publish date approaching without essay drafted

---

## Step 4 — Compose the Output

**TEA Business Pulse — {date}**

**TL;DR:** {1–2 sentence summary. What's working, what needs attention, what's the #1 priority.}

---

**🟢/🟡/🔴 Content Pipeline**
- Queue: {X items ready to produce · X items in draft · X overdue}
- Next essay: {topic or "not yet planned"}
- Saturday batch: {protected / unprotected / partial}

**🟢/🟡/🔴 Course — AI Storyteller's Blueprint**
- Status: {current module and state}
- Next step: {specific action}
- Blocker: {if any}

**🟢/🟡/🔴 Week Ahead**
- {Key calendar commitments this week}
- {Any deadlines or launch dates}

**🟢/🟡/🔴 Urgent Flags**
- {Named items needing action — specific, not generic}

**#1 Priority Today**
{One specific, actionable thing. Not a category — a task. E.g., "Draft the Module 4 intro script — it's been blocked for 10 days and is the current course bottleneck."}

---

*Note: {list any connectors that were unavailable}*

---

## Writing Rules

- Numbers and specifics lead. "3 items in queue" beats "pipeline looks healthy."
- Name the thing. "Module 4 intro script" beats "course content."
- Every flag has a next step — not just an observation.
- No filler. If a section has nothing to report, write "No material changes" and move on.
- Do not invent or estimate. If a source returned nothing, say "n/a."

---

## Scope Variants

- **"Just content"** → Content Pipeline + Saturday Batch only
- **"Just course"** → Course section + any course-related flags
- **"Quick snapshot"** → TL;DR + #1 Priority only
- **"Week ahead"** → Calendar section + any deadline flags

---

## After the Pulse

Offer once:
- "Want me to save this to Notion or Drive?"
- "Want me to post this somewhere?"

If yes, do it. If no or no response, move on — don't ask again.

---

## Reference Files

- `reference/thresholds.md` — 🟢/🟡/🔴 cutoffs, customizable as TEA grows
