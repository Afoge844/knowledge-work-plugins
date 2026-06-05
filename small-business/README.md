# TEA Business Operations Plugin

Pre-built workflows for **The Experience Advantage** — Art Fogelstrom's encore entrepreneurship brand. Built on the Anthropic small-business plugin foundation and customized for a digital-first content and education business.

Install it once and you get a router that understands plain English, TEA-specific skills, and the original small-business building blocks — all wired to Art's actual tool stack.

> **Important**: This plugin assists with business operations and content workflows. All outputs should be reviewed through Art's voice checkpoint (oJoy/Project Shepard) before publishing.

---

## TEA Tool Stack

| Tool | Role | MCP Status |
|---|---|---|
| Notion | Content planning, SOPs, project management | ✅ Connected |
| Gmail | Email, subscriber communications | ✅ Connected |
| Google Calendar | Scheduling, batch day blocking | ✅ Connected |
| Google Drive | Asset storage, 10-folder system | ✅ Connected |
| Canva Pro | Design — carousels, graphics, thumbnails | ✅ Available |
| Fireflies | Meeting/call transcripts | ✅ Connected |
| GitHub | Skills repo, Claude Code workflows | ✅ Connected |
| Rainmaker / GHL | CRM, email automation, funnels | 🔧 Configure endpoint |
| Facebook Pages | Social distribution | ✅ Available |

---

## TEA-Specific Commands

Say these in plain English — the router figures it out.

### Content & Production

| Command | What it does | Just say... |
|---|---|---|
| `/saturday-batch` | Full Saturday content production plan: what to record, what to write, in what order, with time blocks | "what should I produce Saturday", "batch day plan", "Saturday content" |
| `/substack-prep` | Newsletter essay → 21 Notes + derivative assets pipeline | "prep this week's newsletter", "Substack batch", "transform my essay" |
| `/content-repurpose` | One piece of content → full multi-platform asset set | "repurpose this", "turn this into assets", "anchor to asset" |
| `/weekly-engine` | Full weekly content engine run: essay → all derivatives → scheduled | "run the weekly engine", "content week", "full content batch" |

### Community & Business

| Command | What it does | Just say... |
|---|---|---|
| `/skool-pulse` | Skool community health: engagement, new members, tier breakdown, top posts | "how's the community", "Skool check", "community pulse" |
| `/monday-brief` | Week-ahead briefing: Calendar, Notion tasks, content due, community watch | "Monday brief", "start of week", "what's on my plate" |
| `/friday-brief` | End-of-week pulse: wins, content performance, community activity | "Friday recap", "how'd the week go", "end of week" |

### Course & Offers

| Command | What it does | Just say... |
|---|---|---|
| `/course-check` | AI Storyteller's Blueprint module status: what's done, what's next, blockers | "course status", "where am I on the course", "module check" |

---

## Getting Started

Say **"set me up"** or **"get me started"** to run the TEA onboarding skill. It will:
1. Confirm which tools are connected
2. Capture your TEA business context
3. Run a demo pulse using your live data
4. Set your weekly check-in cadence (default: Monday morning)

---

## Customizing Further

- **Add thresholds** — edit `skills/business-pulse/reference/thresholds.md` for your Skool member counts and Substack subscriber milestones
- **Add brand voice** — `skills/tea-onboard/reference/` contains Art's brand voice doc
- **Extend the router** — edit `skills/tea-router/SKILL.md` to add new commands as TEA grows
