# CGA Onboarding Flow

This script runs on first invocation of /cga when no business environment exists. It builds the per-business environment at ~/.claude/cga/{business-slug}/.

## Before You Begin

Check if a business environment already exists:
1. Look for directories in ~/.claude/cga/
2. If one or more exist, ask: "I found existing business profiles: {list}. Do you want to work with one of these, or onboard a new business?"
3. If none exist, proceed with onboarding.

---

## Phase 1: Company Identity

Ask these questions ONE AT A TIME. Wait for each answer before asking the next.

**Q1:** "What's your business name?"
→ Generate slug from this (lowercase, hyphens, no special chars). This becomes the directory name.

**Q2:** "What industry are you in? (e.g., SaaS, ecommerce, agency, local services, creator, marketplace)"

**Q3:** "What stage is the business at?"
- Pre-launch (no revenue yet)
- Early (under $10k/mo)
- Growth ($10k-$100k/mo)
- Scale ($100k+/mo)

**Q4:** "In one sentence, what do you sell and who do you sell it to?"

**Q5:** "What's your approximate monthly revenue? (Ballpark is fine — this calibrates the size of plays I'll recommend)"

**Q6:** "How would you describe your brand voice? Pick the closest or describe your own:"
- Professional & polished
- Scrappy & startup-y
- Bold & irreverent
- Technical & precise
- Warm & personal
- Other: ___

**Q7:** "Do you have a logo file I can use for your dashboard? (Paste a path or URL, or skip)"

→ After Phase 1, write company-profile.md:

```
# Company Profile: {Business Name}

- **Slug:** {slug}
- **Industry:** {industry}
- **Stage:** {stage}
- **Offering:** {what they sell + who}
- **Monthly Revenue:** {revenue}
- **Brand Voice:** {voice}
- **Logo:** {path or "none"}
- **Onboarded:** {YYYY-MM-DD}
```

---

## Phase 2: Growth Audit

**Q8:** "What's currently working for growth? What channels bring in customers today?"

**Q9:** "What have you tried that DIDN'T work? (Knowing what failed is as valuable as what succeeded)"

**Q10:** "What's your #1 growth bottleneck right now?"
- Not enough traffic / awareness
- Traffic but low conversions
- Customers but they don't stick (retention)
- Customers who stick but don't refer others
- Not sure — need diagnosis

**Q11:** "When a new customer joins, do they bring anyone else? Is there any referral or word-of-mouth loop happening naturally?"

**Q12:** "Do you have any automated growth loops running already? (e.g., referral programs, automated email sequences, content flywheels)"

→ After Phase 2, write growth-audit.md:

```
# Growth Audit: {Business Name}

## What's Working
{Q8 answer}

## What's Been Tried & Failed
{Q9 answer}

## Primary Bottleneck
{Q10 answer}

## Current Viral Coefficient
{Q11 answer — assess if K > 1, K = 1, or K < 1}

## Existing Growth Robots
{Q12 answer}

## Audit Date: {YYYY-MM-DD}
```

---

## Phase 3: Tool Stack & Integrations

"Now I need to understand your tool stack so I can connect to your data. For each category, tell me what you use (or 'none'):"

Ask these as a batch (not one at a time — too slow):

| Category | Question |
|----------|----------|
| CRM | "What do you use to manage leads/customers?" |
| Revenue/Billing | "What handles your payments/invoicing?" |
| Analytics | "How do you track website traffic?" |
| Email | "What's your email marketing platform?" |
| Ads | "Do you run paid ads? Where?" |
| Social | "Which social platforms are you active on?" |
| Design | "What do you use for creative/design work?" |
| Project Management | "Where do you track tasks and projects?" |
| Cold Outreach | "Do you do outbound? What tool?" |
| Scheduling | "Calendar/scheduling tool?" |

For each tool they name:
1. Check if a matching MCP server is available in the current Claude session
2. If yes: note it as "Connected" in integrations.md
3. If no: note it as "Manual — no MCP available"

→ After Phase 3, write integrations.md:

```
# Integrations: {Business Name}

| Category | Tool | MCP Status |
|----------|------|------------|
| CRM | {tool} | {Connected / Manual} |
| Revenue | {tool} | {Connected / Manual} |
| Analytics | {tool} | {Connected / Manual} |
| Email | {tool} | {Connected / Manual} |
| Ads | {tool} | {Connected / Manual} |
| Social | {platforms} | {Connected / Manual} |
| Design | {tool} | {Connected / Manual} |
| PM | {tool} | {Connected / Manual} |
| Outreach | {tool} | {Connected / Manual} |
| Calendar | {tool} | {Connected / Manual} |

## Integration Notes
{Any special notes about tool configuration or access}
```

---

## Phase 4: Dashboard Deployment

**Q:** "Where would you like your Growth Cockpit dashboard deployed?"
- **Vercel** — I'll scaffold a Next.js app and deploy it. You'll get a live URL.
- **Local HTML** — I'll generate a self-contained dashboard you can open in your browser.
- **Skip for now** — Set up the dashboard later.

If they choose Vercel or Local, proceed with dashboard scaffolding (detailed in Plan 4).
If they skip, note it in the environment and move on.

→ Note dashboard preference in company-profile.md (append):
```
- **Dashboard:** {vercel / local / skipped}
- **Dashboard URL:** {url or "pending"}
```

---

## Phase 5: Create Remaining Environment Files

After all questions are answered, create the remaining environment structure:

```bash
mkdir -p ~/.claude/cga/{slug}/growth-robots/{active,proposed}
mkdir -p ~/.claude/cga/{slug}/experiments
```

Create tactic-board.md:
```
# Tactic Board: {Business Name}

## Proposed
(No plays yet — run a diagnosis to generate initial recommendations)

## Approved

## Active

## Measuring

## Completed

## Declined
```

Create growth-robots/inventory.md:
```
# Growth Robot Inventory: {Business Name}

## Active Robots
(None yet)

## Proposed Robots
(None yet — run a diagnosis to identify loop opportunities)

## Retired Robots
(None)
```

Create growth-log.md:
```
# Growth Log: {Business Name}

## {YYYY-MM-DD} — Onboarded
- Business profiled and environment created
- Tool stack mapped: {count} integrations ({connected_count} connected via MCP)
- Primary bottleneck identified: {bottleneck}
- Dashboard: {status}
```

Create chat-memory.md:
```
# Growth Chat Memory: {Business Name}

## User Preferences
(Learned through conversation — updated by Growth Chat)

## Key Decisions
(Logged as the CEO makes approval/decline decisions)

## Insights
(Patterns noticed over time)
```

Create empty experiments/ directory.

---

## Phase 5B: Initial Diagnosis

After environment creation, run a quick first-pass diagnosis:

1. Review the growth audit (bottleneck, what's working, what failed)
2. Review the tool stack (what data is available)
3. Based on the bottleneck, propose 3 initial growth plays:
   - 1 WHITE hat play (safe, immediate)
   - 1 GREY hat play (higher impact, requires approval)
   - 1 growth robot concept (a loop, not a campaign)

Present these in the terminal with the approval gate format:
```
Here are your first 3 growth plays based on the audit:

1. [WHITE] {Play name} — {one-line summary}
2. [GREY] {Play name} — {one-line summary}
3. [ROBOT] {Robot name} — {one-line summary of the loop}

Would you like to approve any of these, get more detail, or ask the Growth Chat for alternatives?
```

Add proposed plays to tactic-board.md under "Proposed."

---

## Onboarding Complete Message

```
Your CGA environment is ready.

Business: {name}
Environment: ~/.claude/cga/{slug}/
Integrations: {count} tools mapped ({connected} via MCP)
Bottleneck: {bottleneck}
Initial plays: 3 proposed (check your tactic board)

Run /cga anytime to enter operational mode. I'll load your profile and we'll hunt for growth robots.
```

---
