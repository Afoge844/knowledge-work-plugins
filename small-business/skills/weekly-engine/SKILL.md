---
name: weekly-engine
description: >
  Runs Art's full weekly content engine in one session. Pulls the Notion content
  queue, identifies this week's anchor piece, runs the Anchor-to-Asset
  transformation, organizes all assets into a publishing schedule, and updates
  Notion with statuses. The end state: a complete week of content across all
  platforms, ready for voice checkpoint, organized and scheduled.
  Use when Art says "run the weekly engine", "full content batch",
  "content week", or "set up the whole week."
---

# Weekly Engine

This is the full weekly content production run. One command drives the entire pipeline from queue to publishing-ready assets. Art approves at two checkpoints — nothing publishes without his say-so.

## What This Does

1. Pulls current content queue from Notion
2. Selects the anchor piece for the week
3. Runs Anchor-to-Asset transformation (all 7+ derivative assets)
4. Builds a platform-by-platform publishing schedule
5. Updates Notion queue statuses
6. Surfaces voice checkpoint reminder

Estimated time: 20–30 minutes total (mostly waiting for Claude to build assets).

---

## Step 1 — Pull Queue and Select the Anchor

Query Notion for all content items. Identify:
- What's "Ready to Publish" (most urgent — already produced, needs assets)
- What's "Ready to Record" (this week's production candidate)
- What's overdue

**Anchor selection logic:**
1. If there's a completed essay or recording ready → that's the anchor
2. If not, pick the highest-priority item from "Ready to Record" and note it needs production first
3. If nothing is queued → flag it and ask Art: "Your queue is empty. What topic do you want to build this week around?"

Present the anchor selection: "This week's anchor piece: [title/topic]. Confirm or swap?"

**Checkpoint 1: Art confirms the anchor before any assets are built.**

---

## Step 2 — Run Anchor-to-Asset Transformation

Once anchor is confirmed, run the full asset build using the `substack-prep` or `content-repurpose` skill depending on content type:

- **If anchor is a newsletter essay** → run `substack-prep` (full 21 Notes + all 7 assets)
- **If anchor is a podcast or video** → run `content-repurpose` (8 assets)
- **If anchor is a course lesson recording** → run `content-repurpose` with course-specific clip selection

Output: all assets labeled and organized by platform.

---

## Step 3 — Build the Publishing Schedule

Organize all assets into a 7-day posting calendar. Use TEA's standard publishing cadence:

| Day | Platform | Asset |
|---|---|---|
| Sunday | Substack | Newsletter essay (if publish day is Sunday) |
| Monday | LinkedIn | Long-form post |
| Monday | Substack Notes | Note 1 of 7 |
| Tuesday | Substack Notes | Note 2 of 7 |
| Tuesday | Facebook | Facebook post |
| Wednesday | LinkedIn | Carousel (Art produces in Gamma from outline) |
| Wednesday | Substack Notes | Note 3 of 7 |
| Thursday | Short-form video | TikTok / Reels / Shorts clip |
| Thursday | Substack Notes | Note 4 of 7 |
| Friday | Email list | Broadcast via Rainmaker/GHL |
| Friday | Substack Notes | Note 5 of 7 |
| Saturday | Skool | Community prompt |
| Saturday | Substack Notes | Notes 6–7 of 7 |

Adjust based on Art's actual Substack publish day and any confirmed Calendar commitments.

Output as a clean table: Day · Platform · Asset · Status (Draft / Ready for Voice Check / Scheduled).

---

## Step 4 — Update Notion

After Art reviews and approves the schedule:

**Checkpoint 2: Art confirms the publishing schedule before Notion is updated.**

With approval, update Notion:
- Move anchor piece status to "Assets Complete — Voice Check Pending"
- Add publishing dates to each content item
- Create a new Notion page or update the weekly content tracker with the full asset set

If Notion is not connected, output the full schedule as a structured document Art can paste into Notion manually.

---

## Step 5 — Voice Checkpoint Reminder

End every weekly engine run with:

> "Full week is staged. Before anything goes live, run the assets through oJoy/Project Shepard. That's your quality gate — don't skip it."

---

## Guardrails

- **Two checkpoints — anchor confirmation and schedule confirmation.** Nothing moves forward without explicit approval at each.
- **Never post or schedule directly to any platform.** This skill stages content, not publishes it.
- **Saturday is the production day.** If Art is running the weekly engine mid-week, note what's ready now vs. what needs Saturday production first.
- **Voice checkpoint is non-negotiable.** Always include the reminder. Never suggest assets are "ready to post" — always "ready for voice checkpoint."
- **One anchor per week.** Do not try to build assets for two different source pieces in one weekly engine run.
