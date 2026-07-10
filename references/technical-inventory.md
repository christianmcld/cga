# CGA Technical Inventory — MCP Servers, APIs & Tools

**Purpose:** The CGA's technical knowledge of what's available for building growth robots. Updated weekly.
**Last updated:** 2026-07-10

---

## Week of 2026-07-10 — Recon Summary

**Major finds this week:** MCP spec 2026-07-28 RC drops — stateless protocol, MCP Apps (server-rendered UIs), Tasks extension, formal 12-month deprecation policy. Five new MCP servers confirmed: Meta Ads (official, 29 tools), Calendly (official, 35 tools, hosted), ClickUp (official public beta, all plans), Postmark by ActiveCampaign (24 tools, open source). Meta comprehensive community MCP at 200+ tools. OpenAI deprecation wave accelerating: `gpt-4`, `o1`, `gpt-3.5-turbo`, `o3-mini`, `o4-mini` all killed Oct 23, 2026. Claude API rate limits raised — Sonnet/Haiku now match Opus; `claude-opus-4-7` fast mode deprecated July 24. LinkedIn native vertical video getting 38% engagement / 42% visibility boost. X article links from Substack/Medium now specifically boosted by Grok-powered feed.

---

## Week of 2026-07-03 — Recon Summary

**Major finds this week:** 11 brand-new MCPs launched since January 2026 (GHL official, Shopify suite, Airtable, Beehiiv, Twilio, AWS, Atlassian, X/Twitter, TikTok Ads, Salesforce hosted, Instantly.ai). MCP ecosystem now at 2,000+ servers globally. LinkedIn algorithm now heavily penalizes carousels in favor of native text. X API restructure makes URL posts cost $0.20/each and locks follows/likes behind Enterprise. Instagram Plus ($3.99/mo) launched May 2026.

---

## MCP Servers Available (Claude.ai + Local)

These are live connections the CGA can use during sessions to pull data, push content, and build robots.

### Data & Analytics
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Stripe** | Payment data, subscriptions, customers, invoices, revenue | Revenue tracking, churn detection, LTV calculation, abandoned cart data | Native |
| **Google Calendar** | Events, scheduling, free time | Book meetings, event-based robots | Native |
| **Gmail** | Read/search emails, create drafts | Email monitoring, outreach automation | Native |
| **Notion** | Pages, databases, comments, search | Project management, CRM, content planning | Native |
| **Google Analytics (GA4)** ⭐ NEW | GA4 sessions, pageviews, events, conversions, custom reports | Traffic analysis, conversion tracking, funnel analysis | `npx -y google-analytics-mcp` |
| **Google Search Console** ⭐ NEW | Search queries, CTR, impressions, striking-distance keywords, cannibalization detection | SEO robot — keyword gap analysis, CTR optimization | `npx -y mcp-server-gsc` |
| **Ahrefs** ⭐ NEW | Keyword research, backlinks, domain ratings, SERP positions, content gap | SEO analysis, competitor research, link-building automation | `npm install -g @ahrefs/mcp` (official) |
| **Semrush** ⭐ NEW | Keyword overview, domain analytics, backlink data, position tracking | Competitive SEO research, keyword monitoring | `npx -y github:mrkooblu/semrush-mcp` |

### CRM & Sales Intelligence
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Calendly** ⭐ NEW (OFFICIAL) | 35 scheduling and org-management tools — availability, event types, booking, meeting management. Fully hosted by Calendly. OAuth 2.1 + Dynamic Client Registration (no pre-registration needed) | Meeting booking robot, availability management, event type automation, org-wide scheduling workflows | Remote hosted: `https://mcp.calendly.com` (GA Feb 2026, announced Mar 11, 2026) |
| **GoHighLevel (GHL)** ⭐ NEW (OFFICIAL) | Contacts, calendar, conversations, opportunities, payments, sub-accounts — full CRM | Full CRM automation, pipeline robots, SMS/email from AI, location management | Remote: `https://services.leadconnectorhq.com/mcp/` (free on Unlimited+ plans) |
| **HubSpot** ⭐ NEW | Contacts, companies, deals, tickets, notes, lists — read + write | Lead management, deal tracking, contact enrichment, CRM robots | Remote OAuth: `https://mcp.hubspot.com` (GA Q4 2025) |
| **Salesforce** ⭐ NEW | Accounts, opportunities, leads, contacts, custom objects, SOQL queries | Enterprise CRM automation, pipeline management | Remote: enable in Salesforce Setup; or `npx @salesforce/mcp` (GA April 2026) |
| **Apollo.io** ⭐ NEW | Prospect search, contact enrichment, company enrichment, sequences, outreach tracking — 45 tools | Lead mining, contact enrichment, outreach sequencing | `npx -y @inferensys/apollo-io-mcp` (free tier available) |

### Email, Outreach & Messaging
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Postmark (by ActiveCampaign)** ⭐ NEW (OFFICIAL) | 24 tools: single + batch email sending (up to 500/call), template CRUD + validation, message search, delivery diagnostics (diagnoseDelivery tool), bounce management, suppression lists, webhooks, server info. Open source MIT. | Transactional email robot — send AI-drafted emails, diagnose deliverability, manage templates, bulk sends | Clone: `github.com/ActiveCampaign/postmark-mcp` (requires Postmark API key) |
| **Klaviyo** | Email marketing, campaigns, segments, profiles | Email robots, list management, campaign automation | Native |
| **Beehiiv** ⭐ NEW | Subscriber analytics, publication stats, post management, audience segmentation | Newsletter growth robot, audience analysis, post scheduling | Remote OAuth (enable in Beehiiv settings); or `npx -y beehiiv-mcp-server` (GA March 2026) |
| **Instantly.ai** ⭐ NEW | Campaigns, leads, accounts, analytics — 31 tools | Cold email robot — create campaigns, add leads, track performance | `pip install instantly-mcp` (requires Instantly API key) |
| **Twilio** ⭐ NEW | SMS, voice, phone numbers, verify, conversations — 1,800+ endpoints | SMS outreach robots, OTP flows, conversation automation | `npx -y @twilio/mcp-server` or Claude Code `/plugins` → "twilio-developer-kit" (Public Beta 2026) |
| **SendGrid** ⭐ NEW | Contact lists, email templates, single sends, campaign stats, suppression lists | Email campaign automation, transactional email robots | `npx -y sendgrid-mcp` (set `SENDGRID_API_KEY`) |
| **Slack** | Messaging (authenticate first) | Team notifications, alerts | Native |

### Content & Creative
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Canva** | Design creation, templates, brand kits, export | Ad creative generation, social graphics, lead magnets | Native |
| **Figma** | Design files, components, screenshots | Landing page design, UI mockups | Native |
| **Gamma** | AI presentations, documents, webpages | Pitch decks, lead magnets, content | Native |
| **Hugging Face** | AI models, datasets, papers | Custom AI tools, content generation | Native |
| **fal.ai** ⭐ NEW | 600+ AI models — image gen (Flux/SDXL), video gen, speech-to-text, music, upscaling | Visual content robots, ad creative generation, video production pipeline | `npx -y fal-ai-mcp` (set `FAL_KEY`; or `claude mcp add fal-ai -e FAL_KEY=your-key -- npx -y fal-ai-mcp`) |

### Social Media
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Meta Ads (Official)** ⭐ NEW (OFFICIAL) | 29 tools — campaign creation/management, ad groups, creatives, audience targeting, catalog management, performance analytics, insights. Standard Business OAuth. Open beta as of Apr 29, 2026. Works across Facebook + Instagram Ads Manager. | Full Meta Ads robot — create campaigns, manage budgets, monitor ROAS, generate creative variations, audience management | Remote: Meta Ads Connectors in Business Suite (no developer app needed); or community: `github.com/pipeboard-co/meta-ads-mcp` |
| **Meta Comprehensive (Community)** ⭐ NEW | 200+ tools: Facebook Pages, Instagram, Threads, Ads Manager, Commerce, Conversions API, Custom Audiences, Insights, Ad Library | Full Meta platform robot — organic + paid, organic posting on Pages/IG/Threads plus ad ops in one server | `github.com/oliverames/meta-mcp-server` (community, MIT) |
| **X (Twitter)** ⭐ NEW (OFFICIAL) | 200+ endpoints — search, timelines, user lookups, DMs, lists (read-heavy; write endpoints NOT exposed) | Social listening, trend monitoring, audience research. Note: cannot post via this MCP | Remote OAuth: `https://developer.x.com/en/products/x-api/mcp` (Launched June 30, 2026) |
| **TikTok Ads** ⭐ NEW | Campaign management, ad groups, creatives, audience targeting, performance analytics | TikTok ad campaign robot, performance monitoring, creative management | `pip install tiktok-ads-mcp` (requires TikTok Business API access) |
| **Reddit** ⭐ NEW | Read subreddits, posts, comments, search, user profiles, hot/new/top feeds | Community monitoring, trend detection, social listening robot | `npx reddit-mcp-server` (requires Reddit API credentials) |
| **Ayrshare** ⭐ NEW | 75+ tools across 13 platforms (X, FB, IG, LI, TikTok, YouTube, Pinterest, Reddit, Threads, Bluesky, more) | Multi-platform posting robot, analytics, comment management — one server for all social | `npx -y @ayrshare/mcp-server` (requires Ayrshare API key) |

### Ecommerce
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Shopify** ⭐ NEW (SUITE of 4) | **Storefront**: product catalog, cart, policies; **Customer Accounts**: orders, returns, tracking; **Admin**: full store ops; **Dev**: GraphQL schema | Full Shopify automation — catalog management, order robots, customer service, inventory | Remote hosted (add Shopify MCP endpoint); Community: `npx -y @geli2001/shopify-mcp` (MIT, April 2026) |

### Project Management
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **ClickUp** ⭐ NEW (OFFICIAL, PUBLIC BETA) | Task management with assignees/priorities/due dates, time tracking (start/stop timers, log entries), Docs read/write, comment summarization, executive report generation. Available on all plans. Rate limits: 50 calls/24h (Free), 300 calls/24h (Unlimited+); unlimited with Everything AI add-on. | Project management robot, release notes, status reports, task creation from AI conversations, time tracking | In-app: ClickUp Settings → Integrations → MCP; or `claude mcp add clickup` pointing to ClickUp's hosted endpoint |
| **Atlassian (Jira + Confluence + Bitbucket)** ⭐ NEW | Rovo search across Jira/Confluence, create/update issues and epics, Confluence pages, semantic search | Project management robot, issue tracking, documentation automation | Remote OAuth: `https://mcp.atlassian.com` (GA Feb 4, 2026; free for all Atlassian Cloud customers) |

### Infrastructure & Deployment
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **DigitalOcean** | App deployment, hosting, management | Deploy dashboards, landing pages, tools | Native |
| **Stitch** | UI design system generation | Dashboard and tool UI creation | Native |
| **Cloudflare** ⭐ NEW | 2,500+ endpoints — DNS, Workers, R2 storage, Pages, Zero Trust, KV, D1, WAF | Full infrastructure automation, edge function deployment, CDN management | Remote OAuth: `https://mcp.cloudflare.com`; or `npx -y @cloudflare/mcp-server` |
| **Vercel** ⭐ NEW | Projects, deployment status, env vars, domains, logs, team settings | Deployment robot, env var management, monitoring | `claude mcp add --transport http vercel https://mcp.vercel.com` (OAuth, no local install) |
| **AWS** ⭐ NEW (OFFICIAL) | Full AWS API — CloudFormation, ECS, S3, Lambda, IAM, CDK, docs, cost management | Cloud infrastructure automation, serverless deployment, cost monitoring | `pip install awslabs.core-mcp-server` (GA May 2026; uvx recommended) |
| **Firebase** ⭐ NEW | Firestore, Auth, Storage, Functions, Hosting, Realtime DB — full read/write | Database robots, user management, serverless automation | `npx -y firebase-tools@latest mcp` (built into firebase-tools CLI) |

### Automation & Workflow
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **n8n** ⭐ NEW | Trigger existing workflows, build/edit workflows (v2.13+), all n8n nodes accessible | AI-triggered automation robot — kick off any n8n workflow from Claude | Built-in to n8n — enable in settings, point MCP client at n8n instance URL |

### Web & Research
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Firecrawl** | Web scraping, crawling, search, extraction | Competitor analysis, data scraping, content extraction | Native |
| **Apify** | Web scraping actors, data extraction at scale | Social media scraping, directory scraping, lead mining | Native |
| **Context7** | Library/framework documentation lookup | Technical research for robot building | Native |
| **Playwright** | Browser automation, screenshots, form filling | Web testing, data extraction, automation | Native |

### Productivity & Workspace
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Google Workspace (Full Suite)** ⭐ NEW | Gmail + Drive + Docs + Sheets + Slides + Calendar + Forms + Tasks + Contacts + Chat | Full G-Suite robot — auto-generate docs, update sheets, manage Drive, all in one server | Community (production-ready): `npx -y google-workspace-mcp`; Official preview: Google Workspace Admin Console (Google Cloud Next 2026) |

---

---

## MCP Protocol — 2026-07-28 Release Candidate (Spec Changes)

> **Shipping July 28, 2026.** Biggest spec revision since MCP launched. Affects how servers are deployed and what capabilities they can expose.

| Change | What It Means | Action Required |
|--------|--------------|-----------------|
| **Stateless protocol core** | `Mcp-Session-Id` header removed; `initialize/initialized` handshake eliminated. Client capabilities travel inline in `_meta` field on each request | Servers can now run behind plain round-robin load balancers — no sticky sessions, no shared session stores |
| **MCP Apps (SEP-1865)** | Servers can ship interactive HTML UIs rendered in sandboxed iframes inside the host client. Tools declare UI templates ahead of time for caching/security review | New surface: build dashboards, data entry forms, and rich UIs delivered via MCP — not just text output |
| **Tasks Extension** | Replaces the experimental Tasks core feature from 2025-11-25. `tools/call` can return a task handle; client drives with `tasks/get`, `tasks/update`, `tasks/cancel` | Build long-running robots (crawls, batch sends, report generation) with proper lifecycle management |
| **Extensions Framework** | New capabilities ship as opt-in extensions before (possibly never) moving into the spec core | Watch extension registry for community-built extensions like payments, streaming, specialized tool types |
| **Deprecation Policy** | Formal 12-month deprecation lifecycle: Active → Deprecated → Removed. Three features entering deprecation now: Roots (replaced by tool params), Sampling (call LLM API directly), Logging (use stderr or OpenTelemetry) | Stop using MCP Sampling; stop relying on Roots; route logs to stderr or OTel |
| **Authorization hardening** | OAuth + OIDC alignment; Dynamic Client Registration (RFC 7591) becomes standard pattern | Self-registering clients (no pre-registered app IDs) are now the norm — see Calendly MCP as example |

---

## API Keys Available (Local)

| API | Key Status | What It Enables |
|-----|-----------|-----------------|
| **DigitalOcean** | Active | Deploy apps, manage infrastructure |
| **Firecrawl** | Active | Web scraping and data extraction |
| **Apify** | Active | Scalable web scraping actors |
| **GoHighLevel** | Active | CRM, SMS, email, funnels, automations (Location: y4CP5e3nSzexm2JrnKch) |
| **OpenAI** | Active | GPT for content generation, embeddings |
| **Vercel** | Active | Deploy Next.js apps (dashboards, landing pages, tools) |
| **Stitch** | Active | UI design generation |
| **FAL** | Active | Image/video AI generation |
| **Google AI Studio** | Active | Gemini models, Nano Banana image gen |
| **Stripe** | Active (Live) | Payment processing, subscription management |
| **Plaid** | Pending (dev access) | Bank account connections, expense tracking |

---

## Critical API Deprecations & Shutdowns (Week of 2026-07-10)

> New entries this week:

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **OpenAI `computer-use-preview`** | Shut down | **Jul 23, 2026** | Remove from any automation using this model |
| **OpenAI `gpt-4`, `gpt-3.5-turbo`, `o1`, `o3-mini`, `o4-mini`** | API access removed — calls return errors after deadline | **Oct 23, 2026** | Migrate to GPT-4.1, o3, or o4 now; audit all routing configs |
| **OpenAI older GPT-5 + o3 snapshots** | Deprecated Jun 11, 2026; removed Dec 11, 2026 | **Dec 11, 2026** | Pin to latest stable snapshot IDs, not dated snapshots |
| **Claude Opus 4.7 fast mode** | `speed: "fast"` parameter on `claude-opus-4-7` deprecated | **Jul 24, 2026** (removal) | Remove `speed: "fast"` from any claude-opus-4-7 calls |
| **Wikimedia Core API (`api.wikimedia.org`)** | Gradual deprecation begins Jul 2026; new replacement URLs being created | **Jul 2026 – Jun 2027** | If scraping Wikipedia, switch to new endpoint URLs when published |
| **MCP Roots capability** | Entering formal deprecation (12+ months to removal) | **Jul 28, 2026** (deprecation) | Replace with tool parameters or server config |
| **MCP Sampling capability** | Entering formal deprecation (12+ months to removal) | **Jul 28, 2026** (deprecation) | Call your LLM provider API directly instead |

---

## Critical API Deprecations & Shutdowns (Week of 2026-07-03)

> These affect active robots. Check before building on these platforms.

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **Reddit unauthenticated .json** | 403 Forbidden with no warning; new app registrations also blocked | May 30, 2026 | Use `reddit-mcp-server` with OAuth or third-party aggregators |
| **Google Custom Search JSON API** | Shutting down; closed to new customers | **Jan 1, 2027** | Migrate to SerpApi / Bright Data ASAP |
| **Google Merchant Content API** | Permanent shutdown | **Aug 18, 2026** | Migrate to new Merchant API v1 |
| **OpenAI Assistants API** | All endpoints removed (entire architecture gone) | **Aug 26, 2026** | Migrate to Responses API + Conversations API |
| **OpenAI DALL-E 2 & DALL-E 3** | Retired from API | May 12, 2026 | Use `gpt-image-2` (launched April 21, 2026) |
| **Google Gemini API — Pro models** | Removed from free tier | Apr 1, 2026 | Downgrade to Flash (still free) or pay |
| **Brave Search API** | Free tier eliminated; metered billing activated | Feb 2026 | Budget for ~$5/1,000 queries or switch to SerpApi |
| **Crunchbase API** | Free tier eliminated | 2025 (ongoing) | Basic $49/mo, Pro $99/mo |
| **Shopify Scripts** | All execution ceased | Jun 30, 2026 | Rebuild as Shopify Functions (WebAssembly) |
| **Google Tenor GIF API** | Full shutdown | Jun 30, 2026 | Use Giphy API instead |
| **X/Twitter API — follows/likes/quote-posts** | Require Enterprise contract ($42K/yr) | Apr 20, 2026 | Remove from any automation or sign Enterprise deal |
| **X/Twitter API — URL posts** | Now cost $0.20/post (was $0.010) | Apr 20, 2026 | Build text-first X posts; include URLs only where necessary |
| **Instagram Basic Display API** | Personal accounts locked out permanently | Dec 2024 (enforced 2026) | Business/Creator accounts only via Graph API |
| **Gemini API key restrictions** | Unrestricted keys rejected; restricted keys required | Jun 19, 2026 (partial) / Sep 2026 (full) | Update key restrictions in Google Cloud Console |

---

## New Free Tools & APIs — Week of 2026-07-10

### Instagram DM Automation — Free Tier Landscape (Clarified)

> ManyChat's free plan was gutted in March 2026 (now 25 contacts, one viral Reel exhausts it in a day). New players have moved in with much more generous free tiers.

| Tool | Free DMs/Month | Key Free Features | Robot Potential |
|------|---------------|-------------------|-----------------|
| **ReplyRush** ⭐ | 1,500/month, no card | Comment-to-DM, story reply, keyword triggers | Highest free volume; best for Reel-driven lead capture |
| **LinkDM** | 1,000/month, no card, no expiry | Comment-to-DM, story reply, keyword automation, core features permanent | Permanent free plan — reliable for sustained robots |
| **CreatorFlow** | 500/month, no card | Comment-to-DM, story replies, keyword triggers, templates, link tracking | Flat $15 upgrade path for 5,000 DMs/month |
| **PostEngage.ai** | Unlimited contacts, no card | Full automation suite on free plan — no contact caps | Best free option if volume is high; unusual unlimited free tier |

**Key Change:** ManyChat is no longer viable for free-tier robots. Route new Instagram DM automation builds to ReplyRush or LinkDM.

### AI Rate Limit Improvements (Claude API — Week of 2026-07-10)

| Change | Detail |
|--------|--------|
| **Sonnet + Haiku rate limits raised to match Opus** | All three model tiers now share the same rate limits at every usage tier (Start, Build, Scale) |
| **Usage tiers consolidated** | Three tiers now: Start, Build, Scale. Most organizations moved to higher tier automatically with no action required |
| **Net effect for robots** | High-volume Claude robots can now use Haiku or Sonnet at the same rate ceiling as Opus — reduces cost for batch operations |

---

## New Free Tools & APIs — Week of 2026-07-03

### Social Publishing APIs (New)
| Tool | Free Tier | Robot Potential | URL |
|------|-----------|-----------------|-----|
| **Buffer API** ⭐ NEW | 100 req/24h, 3 channels, 11 platforms, MCP server included | Cross-platform content distribution robot | buffer.com/api |
| **Publora** ⭐ NEW | 15 posts/mo, 10 platforms, full REST + MCP-native | Agent-first publisher — Claude/GPT posts autonomously | publora.com |
| **Late API** ⭐ NEW | 20 posts/mo, 13 platforms incl. Reddit + Snapchat | Widest platform coverage of any free publisher | getlate.dev |
| **Bluesky AT Protocol** ⭐ NEW | Fully free — no API key, no approval, 5K pts/hr | Only major social with completely open free API | docs.bsky.app |

### AI Inference APIs (Free Tiers)
| Tool | Free Tier | Robot Potential | Notes |
|------|-----------|-----------------|-------|
| **Gemini 2.5 Flash (AI Studio)** | 250 RPD, 15 RPM, 1M token context, no card, no expiry | High-volume content generation, SEO copy at scale | Pro models removed from free tier Apr 1, 2026 |
| **Groq** | 14,400 req/day, 30 RPM, no card, 300+ tok/sec | Real-time outreach personalization; audio transcription (Whisper free) | console.groq.com |
| **Cerebras** | 1M tokens/day, 30 RPM, no card | Highest free daily token volume — bulk content generation | cloud.cerebras.ai |
| **Mistral Codestral** | 2,000 req/day, 30 RPM, no card | Automation scripting, code generation for robots | codestral.mistral.ai |
| **OpenRouter** | 28+ free models, 1M BYOK routing/month | Single API key across 28+ free models with auto-failover | openrouter.ai |
| **Cloudflare Workers AI** | 10,000 neurons/day, Stable Diffusion + Whisper free | Edge-deployed content tools, free image generation | developers.cloudflare.com/workers-ai |

### Scraping & Data APIs (New/Notable)
| Tool | Free Tier | Robot Potential | URL |
|------|-----------|-----------------|-----|
| **ScrapeCreators** | 1,000 credits, no card, no expiry | Reddit/LinkedIn/TikTok scraping for social intelligence | scrapecreators.com |
| **SociaVault** | 50 credits, no card, no expiry | Cross-platform engagement data across 9 networks | sociavault.com |
| **Job Postings API (TheirStack)** | 100K+ calls free, 1.8M US jobs daily | Hiring signals as sales triggers — companies hiring = growth intent | theirstack.com/en/job-posting-api |
| **HasData Google AI Mode API** | 1,000 free calls, no card | Monitor Google AI search answers — SEO intelligence | hasdata.com/apis/google-ai-mode-api |

### Automation Platform Updates (2026)
| Tool | Key 2026 Update | Growth Impact |
|------|-----------------|---------------|
| **n8n** | Multi-agent orchestration, MCP support (v2.28+), AI Agent node with ReAct mode, intelligent model routing (60% cost reduction), ALL active workflow limits removed | Best free self-hosted automation stack for growth robots |
| **Make** | Full AI Agents app (Feb 2026), MCP tools for agents (Jun 2026), Module tools (any Make app as agent tool) | 3,000+ app integrations now available to AI agents |
| **Zapier** | Inline formulas (no more Formatter steps), BYOK AI provider, Agents templates in unified hub, Canvas + Agents | AI Guardrails for compliance (Enterprise only) |

---

## Free Tools & APIs for Robot Building

### Content Creation & Repurposing
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Whisper (local)** | Unlimited (local install) | Audio/video transcription for clipping robots |
| **FFmpeg (local)** | Unlimited | Video editing, metadata manipulation, format conversion |
| **MarkItDown** | Unlimited | Convert any doc to markdown for AI processing |
| **Buffer** | 3 channels free | Social media scheduling |
| **Later** | 1 social set free | Visual social media scheduling |
| **Canva (MCP)** | Connected | Design automation |
| **Unsplash API** | 50 req/hr | Free stock photos for content |
| **Pexels API** | 200 req/hr | Free stock photos + videos |

### Email & Outreach
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Mailchimp** | 500 contacts free | Email marketing starter |
| **Brevo (Sendinblue)** | 300 emails/day free | Transactional + marketing email |
| **Beehiiv** | Free tier with referral program | Newsletter with built-in viral mechanics |
| **ConvertKit** | 1,000 subscribers free | Creator-focused email |
| **Hunter.io** | 25 searches/mo free | Email finder for outreach |
| **Streak (Gmail)** | Free CRM + email tracking | Track opens, gauge interest |
| **YAMM** | 50 emails/day free | Gmail mail merge for mass personalized outreach |

### SEO & Analytics
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Google Search Console** | Free | SEO data, keyword performance, indexing |
| **Google Analytics 4** | Free | Traffic, behavior, conversion tracking |
| **Ubersuggest** | 3 searches/day free | Keyword research |
| **AnswerThePublic** | 1 search/day free | Content idea generation from search queries |
| **Google Trends** | Free | Trend identification for Trend Rider robot |
| **Ahrefs Webmaster Tools** | Free (own site only) | Backlink monitoring, site audit |

### Social Media
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Meta Graph API** | Free | Facebook/Instagram data, posting |
| **LinkedIn API** | Limited free | Profile data, posting (strict limits) |
| **X/Twitter API** | Free tier (read-only) | Monitoring, trend detection |
| **YouTube Data API** | 10,000 units/day free | Video data, comments, search |
| **Pinterest API** | Free | Pin creation, board management |
| **TikTok API** | Free (creator tools) | Video data, trend analysis |
| **Reddit API** | Free (100 req/min) | Monitoring, posting, community engagement |

### CRM & Lead Management
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **GoHighLevel** | Active (via API key) | Full CRM, SMS, email, funnels, automations |
| **HubSpot CRM** | Free forever | Contact management, deal tracking, forms |
| **Notion (MCP)** | Connected | Lightweight CRM, project management |
| **Airtable** | 1,000 records free | Structured data, forms, automations |

### Automation & Integration
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Zapier** | 5 zaps, 100 tasks/mo free | Connect any two tools |
| **Make (Integromat)** | 1,000 ops/mo free | Visual automation builder |
| **n8n** | Self-hosted (free) | Open-source automation, unlimited workflows |
| **GitHub Actions** | 2,000 min/mo free | CI/CD, scheduled scripts, automation |
| **Cron-job.org** | Free | Schedule HTTP requests (trigger webhooks) |
| **IFTTT** | 2 applets free | Simple trigger-action automations |

### AI & Generation
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Claude API** | Pay-per-use | Content generation, analysis, chat |
| **OpenAI API** | Pay-per-use (key active) | GPT for content, embeddings |
| **Google AI Studio** | Free tier generous | Gemini models, multimodal |
| **FAL.ai** | Key active | Image/video generation |
| **Replicate** | Some free models | Run open-source AI models |
| **Hugging Face (MCP)** | Connected | Model inference, spaces |

### Landing Pages & Web
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Vercel** | Free tier (active key) | Deploy Next.js apps, dashboards |
| **Netlify** | Free tier | Static site hosting |
| **Carrd** | Free (1 site) | Simple landing pages |
| **Tally** | Free (unlimited forms) | Form builder, data collection |
| **Typeform** | 10 responses/mo free | Interactive forms and quizzes |

### Review & Reputation
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Google Business Profile API** | Free | Manage reviews, posts, listings |
| **Trustpilot API** | Free tier | Review monitoring |
| **Yelp Fusion API** | 5,000 calls/day free | Business search, reviews |

### Data & Enrichment
| Tool | Free Tier | Robot Potential |
|------|-----------|-----------------|
| **Clearbit** | Limited free | Company/person enrichment |
| **FullContact** | 100 matches/mo free | Contact enrichment |
| **Abstract API** | Various free tiers | Email validation, geolocation, VAT |
| **IPinfo** | 50,000 req/mo free | IP geolocation for visitor intelligence |

---

## Robot-to-Tool Mapping

When building a growth robot, match parts to available tools:

| Robot Part | Primary Tools |
|-----------|--------------|
| **APIs** | Firecrawl, Apify, social platform APIs, Google APIs |
| **Applications** | GoHighLevel, Notion, Canva, Vercel, email platforms |
| **Users** | Forms (Tally/Typeform), CRM (GHL/HubSpot), email capture |
| **Product** | Vercel deployments, web apps, tools, calculators |
| **AI Agents** | Claude API, OpenAI, Gemini, Whisper, FAL |
| **Partnerships** | Email (Beehiiv swaps), affiliate tracking |
| **Automation** | n8n, Make, Zapier, GitHub Actions, cron-job.org |

---

## Weekly Update Protocol

Every week, the CGA should research:
1. New MCP servers available for Claude Code
2. New free APIs launched (Product Hunt, dev newsletters)
3. Platform API changes (rate limits, new endpoints, deprecations)
4. New automation tools with free tiers
5. New AI models that enable new robot capabilities

Update this file and commit to the skill repo.
