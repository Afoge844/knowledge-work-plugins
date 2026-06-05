---
name: saturday-batch
description: >
  Builds Art's Saturday content production plan. Pulls the Notion content queue,
  checks Google Calendar for any conflicts, then outputs a time-blocked
  production schedule optimized for ADHD-aware batch work — one task type at a
  time, no context switching, with clear stop points and a prioritized order.
  Use when Art asks "what should I produce Saturday", "batch day plan",
  "Saturday content", or any variant of planning Saturday's work.
---

# Saturday Batch Skill

Saturday is the anchor day. All creative work concentrates here. This skill makes sure Art walks into Saturday knowing exactly what to produce, in what order, and how long each block takes — so zero mental energy goes to planning during the production day itself.

## Step 1 — Pull Content Queue from Notion

Query Notion for all content items with any of these statuses:
- "Ready to Record"
- "Ready to Write"
- "Draft — Needs Editing"
- "Overdue"
- "This Week"

For each item, capture: title, type (video/podcast/essay/notes/carousel), estimated time, platform target, and any dependencies.

If Notion is not connected, ask Art to paste his current content queue or describe what he has ready to work on.

## Step 2 — Check Calendar for Saturday

Pull Google Calendar for the upcoming Saturday. Flag:
- Any meetings or appointments that will eat into batch time
- Any hard deadlines on Sunday or Monday that make certain content urgent
- Whether a full production block is already scheduled (🟢) or not (🔴)

If no block is scheduled, note it: "Saturday has no production block on Calendar — want me to add one?"

## Step 3 — Assess What's Ready

Before building the plan, determine readiness:

**Ready to record?**
- Script or talking points drafted?
- Recording setup ready (microphone, camera, lighting)?
- Content fully planned or needs more prep?

**Ready to write?**
- Research done?
- Outline exists?
- Any raw material (call notes, Fireflies transcripts, ideas) to draw from?

Pull Fireflies transcripts from the past 7 days — any meeting notes that contain usable content ideas or raw material for the queue?

## Step 4 — Build the Time-Blocked Plan

Output a Saturday production schedule. Rules:
- **One task type per block.** Do not mix recording and writing. Do not mix editing and planning.
- **Hardest/most creative work first** — script writing and recording in the morning
- **Mechanical work last** — editing, formatting, uploading in the afternoon
- **Maximum 90-minute focused blocks** with 15-minute breaks between
- **Stop time matters** — include an end point so the day has a defined finish

**Standard TEA Saturday Block Structure:**

```
SATURDAY BATCH DAY — {date}

MORNING BLOCK (9:00 AM – 12:00 PM)
[90 min] 9:00–10:30 → {Task 1: most cognitively demanding — script, essay draft, or recording prep}
[15 min] 10:30–10:45 → BREAK
[90 min] 10:45–12:15 → {Task 2: recording or primary writing}

AFTERNOON BLOCK (1:00 PM – 4:00 PM)
[90 min] 1:00–2:30 → {Task 3: secondary recording or first edit}
[15 min] 2:30–2:45 → BREAK
[90 min] 2:45–4:15 → {Task 4: mechanical work — editing, captions, upload, scheduling}

WRAP (4:15–4:30 PM)
→ Update Notion queue with status changes
→ Note anything unfinished for next Saturday
→ Batch day complete ✓
```

Populate each block with Art's specific content items from the queue, ordered by urgency and type.

## Step 5 — Flag Dependencies and Blockers

Before presenting the plan, flag anything that could break it:
- Any content item that needs research not yet done → move to "prep for next week"
- Any recording that needs tech setup not confirmed → flag it
- Any item with a Monday deadline → move it to Block 1 regardless of type
- If the queue has < 3 items → note it and suggest what to add based on TEA's content calendar

## Step 6 — Present and Confirm

Show the full plan. Ask: "Does this order work for you, or do you want to swap anything?"

After confirmation, offer:
- "Want me to add these blocks to your Google Calendar?"
- "Want me to update the Notion queue statuses to 'In Progress' for Saturday's items?"

Never add to Calendar or update Notion without explicit confirmation.

## Guardrails

- **Never schedule creative work on non-Saturday days** unless Art explicitly requests it.
- **Voice checkpoint reminder:** Any content produced Saturday goes through oJoy/Project Shepard before publishing. Include this reminder at the end of the plan.
- **Do not overload the day.** If the queue has 8 items but Saturday only has 6 productive hours, prioritize the top 4–5 and move the rest to "Next Saturday."
- **Batch by type.** Never interleave recording and writing tasks in the same block.
