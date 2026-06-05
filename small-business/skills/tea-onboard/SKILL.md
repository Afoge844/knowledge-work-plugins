---
name: tea-onboard
description: >
  TEA-specific onboarding. Confirms connected tools, captures Art's current
  business context (active workstreams, Skool tier counts, Substack subscriber
  count, course module status, current headaches), stores it persistently so
  every other skill benefits, and sets the weekly Monday check-in cadence.
  Use when Art says "set me up", "get started", "what can you do", or is in
  his first session with this plugin.
---

# TEA Onboard

## Quick Start

Four moves: confirm connectors → run one demo skill → capture TEA context → set weekly rhythm. Takes 10–15 minutes. Ends with every skill knowing Art's business.

```
Art: "set me up"
→ Check which connectors are active
→ Run business-pulse with whatever is connected (prove value immediately)
→ Ask 6 TEA-specific questions one at a time
→ Store context to memory
→ "Every Monday, say 'Monday brief' and I'll pull your week ahead."
```

---

## Connector Check

On start, check which of these are active. List what's connected and what's not — one line each. For anything not connected, name **one concrete thing** it would unlock, then move on. Do not push.

| Connector | Unlocks |
|---|---|
| Notion | Saturday batch planning, course status, content queue |
| Google Calendar | Time-blocking, week-ahead view, batch day protection |
| Gmail | Subscriber email signals, urgent flags |
| Google Drive | Asset storage, export to 10-folder system |
| Canva | Carousel and graphic creation from content briefs |
| Fireflies | Auto-pull call/meeting notes into content pipeline |
| Rainmaker/GHL | Lead and subscriber CRM data |
| GitHub | Skills ecosystem status, Claude Code repo tracking |
| Facebook Pages | Distribution tracking |

---

## Demo Skill (Run Immediately After First Connector Confirms)

Do not wait for all connectors. As soon as any one connector is live, run `business-pulse` against it. Narrate what you're doing:

> "Let me show you what this looks like with your live data..."

This is the aha moment. Do not skip it to get to the interview faster.

---

## The Six TEA Interview Questions

Ask one at a time. Wait for the full answer. One follow-up if vague — no more.

1. **Active workstreams.** "What are your top 3 active workstreams right now — the things you're actually working on this week?"

2. **Course status.** "Where are you on the AI Storyteller's Blueprint course? Which modules are complete, which are in progress, and what's the current blocker?"

3. **Platform numbers.** "Give me a quick snapshot of your current numbers: Substack subscribers, Skool members (by tier if you know them), and email list size."

4. **Current headaches.** "What are the two or three things eating your time or keeping you up at night right now — content, tech, business development, community?"

5. **Content queue.** "What's the next newsletter essay topic, and do you have any content already drafted or recorded that needs to be processed?"

6. **Weekly rhythm.** "How do you want me to check in — Monday morning brief only, or also a Friday recap?"

If Art is short on time, compress to questions 1, 4, and 5 — those three feed the most downstream skills.

---

## Context Storage Format

Show the full profile before writing. Wait for explicit approval. Write under `## Business context` in session memory. Do not touch other content.

```markdown
## Business context

- **Business:** The Experience Advantage — encore entrepreneurship brand (AI-powered income streams for professionals 45–65)
- **Active workstreams:** <workstream 1> · <workstream 2> · <workstream 3>
- **Course status:** <module status summary — e.g., "Modules 1–3 complete, Module 4 in progress, blocker: recording setup">
- **Platform numbers:** Substack: <count> · Skool: <count> (<tier breakdown if known>) · Email list: <count>
- **Top headaches:** <headache 1> · <headache 2> · <headache 3>
- **Content queue:** <next essay topic> · <any drafted content ready to process>
- **Connected tools:** <comma-separated active connectors>
- **Weekly cadence:** <Monday brief / Friday recap / both>
- **Voice checkpoint:** oJoy/Project Shepard — mandatory before any content publishes
- **Batch day:** Saturday (protected — all creative production concentrated here)
- **Onboarded:** <YYYY-MM-DD>
```

---

## Approval Gates

- **Show full profile before writing.** Wait for explicit "looks good" or "save it."
- **Never overwrite existing context silently.** If a block exists, show current vs. proposed.
- **Never connect a tool on Art's behalf.** Guide; do not act.

---

## After Onboarding

Confirm: *"Saved. Every skill from here will know your business."*

Then: *"Each Monday, say 'Monday brief' and I'll pull your week ahead — Calendar, Notion tasks, community watch, and your top 3 priorities. Want to try it now, or save it for Monday?"*

If tools are connected, name one skill Art can try right now with its exact trigger phrase.
