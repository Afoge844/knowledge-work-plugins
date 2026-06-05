---
name: skool-pulse
description: >
  TEA Skool community health check. Pulls available community data and produces
  a one-page pulse: new member count, tier breakdown, engagement signals,
  top posts this week, any unanswered questions, and one recommended community
  action for the week. Works with pasted data or Rainmaker/GHL if connected.
  Use when Art asks "how's the community", "Skool check", "community pulse",
  or "how are my members doing."
---

# Skool Pulse

One prompt, one community snapshot. Surface what's happening in the TEA Skool community so Art can engage strategically rather than reactively.

## Input Options

Try in this order:
1. **Rainmaker/GHL** — if connected, pull member data, tier counts, recent activity
2. **Pasted data** — if Art pastes a Skool dashboard screenshot description or export, work from that
3. **Manual input** — ask Art: "Give me a quick rundown: new members this week, any cancellations, and anything you've noticed in the community?"

---

## Step 1 — Pull Community Data

From whatever source is available, gather:

**Membership:**
- Total members (all tiers)
- Tier breakdown: Community-only ($79/mo) · Community + Course ($149/mo) · Founders Annual ($1,497/yr)
- New members this week (WoW count)
- Cancellations or downgrades this week
- Members approaching their first 30 days (at-risk window for early churn)

**Engagement:**
- Posts or questions from members in the past 7 days
- Any posts with no response from Art or the community
- Top-performing post this week (most comments or engagement)
- Any complaints, frustrations, or technical issues raised

**Founders Annual (6 spots):**
- How many of the 6 spots are filled?
- Any Founders due for their 1:1 onboarding call?
- Any Founders who haven't engaged in the past 14 days?

---

## Step 2 — Compute Health Signals

Assign 🟢/🟡/🔴 using the thresholds in `business-pulse/reference/thresholds.md`.

| Signal | What to measure |
|---|---|
| Member growth | New members WoW vs. prior week |
| Churn risk | Cancellations + members in day 1–30 who haven't posted |
| Engagement | Posts per week, Art's response rate to member questions |
| Founders | All 6 spots filled, all onboarding calls completed |

---

## Step 3 — Compose the Output

**TEA Skool Pulse — {date}**

**Community Health:** 🟢/🟡/🔴

---

**Membership**
- Total members: {X}
- Tier breakdown: Community-only {X} · Community+Course {X} · Founders Annual {X}/{6}
- New this week: {+X} ({vs. last week delta})
- Cancellations: {X}
- At-risk (day 1–30, no post yet): {X members — name them if known}

**Engagement This Week**
- Member posts: {X}
- Unanswered questions: {X — list them specifically}
- Top post: "{title or topic}" — {X comments/reactions}

**Founders Annual**
- Spots filled: {X}/6
- Onboarding calls pending: {X}
- Inactive Founders (> 14 days): {names if known}

**Watch List**
- {Specific member or situation needing Art's attention — named, not generic}

**#1 Community Action This Week**
{One specific thing Art should do in the community — reply to a post, reach out to a member, post a prompt, run an event. Specific enough to act on immediately.}

---

## Step 4 — Offer

After presenting:
- "Want me to draft a community post or prompt to boost this week's engagement?"
- "Want me to save this to Notion or Drive?"

---

## Guardrails

- **Name specifics.** "3 unanswered questions" is useless. Name the questions.
- **Founders Annual gets priority attention.** At $1,497/year, these members deserve white-glove tracking.
- **Never post to the community directly.** All community posts require Art's review first.
- **One action recommendation.** Not a list of 5 things — one clear, doable action for the week.
