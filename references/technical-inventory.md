# CGA Technical Inventory — MCP Servers, APIs & Tools

**Purpose:** The CGA's technical knowledge of what's available for building growth robots. Updated weekly.
**Last updated:** 2026-08-14

---

## Week of 2026-08-14 — Recon Summary

**Major finds this week:** Claude Sonnet 5 pricing is now PERMANENTLY frozen at $2/$10 per MTok (Anthropic announced August 11) — the planned September 1 increase to $3/$15 was cancelled. However, Sonnet 5 runs a new tokenizer that produces ~30% more tokens from the same input, which partially offsets the lower per-token price — re-benchmark robot costs. Three critical API deadlines are imminent: **Google Merchant Content API shuts down August 18 (4 days) — emergency still active**; **Anthropic Workbench (legacy) retires August 17 (3 days) — export data NOW or lose all saved prompts/evals**; **OpenAI Assistants API shuts down August 26 (12 days)**. New MCP find: `containers/kubernetes-mcp-server` (v0.0.65, updated August 12) — the most complete K8s/OpenShift MCP available, enables AI-driven cluster management. PulseMCP paused new server submissions through mid-August for platform rework — count stabilized near 22,000+. TikTok Shop shipped five new seller/creator AI tools: AI Dubbing, AI Fashion Video Maker, and List with AI reduce shoppable video production to near-zero effort. X Phoenix algorithm (open-source) received its third major GitHub commit on August 13 — scoring weights unchanged (replies 27x, retweets 20x) but ranking feature set expanded.

---

## Week of 2026-08-07 — Recon Summary

**Major finds this week:** Google Merchant Content API shuts down **August 18 — 11 days from today**: every programmatic ecommerce robot calling the Content API for Shopping starts failing at 00:01 UTC Aug 18. OpenAI Assistants API shuts down **August 26 — 19 days from today** (already logged; treat as active emergency). MCP ecosystem crossed **22,311 servers** (PulseMCP, July 16) with governance transferred to the Linux Foundation's AAIF — signaling enterprise adoption and long-term spec stability. Three new community Substack MCP servers documented: `postcli/substack`, `dkships/substack-publisher-mcp`, and `marcomoauro/substack-mcp` — covering analytics, drafts, posts, and Notes automation. YouTube surfaced two new algorithm signals: non-subscriber reach (60%+ non-subscriber impressions is the healthy benchmark) and a Browse feed personalization overhaul (micro-niche watch history clustering, February 2026). Instagram confirmed Replace Audio feature (July 21) — swap music on published posts/carousels with zero engagement loss. LinkedIn's 60% external-link reach penalty confirmed by Forbes (July 30) — zero-click native content strategy is now mandatory. X engagement velocity now has a confirmed 30-minute amplification window (10+ engagements triggers distribution). YouTube will also stop push notifications for inactive subscribers — channels with stale follower bases lose their notification reach.

---

## Week of 2026-07-31 — Recon Summary

**Major finds this week:** MCP 2026-07-28 spec officially shipped July 28 — stateless core is live, 400M+ monthly SDK downloads, 10,000+ servers in production; Claude now supports the new spec across all Claude products. Claude Opus 5 launched July 24 at $5/$25 per MTok — near-Fable-5 intelligence at half the price; Sonnet 5 introductory pricing $2/$10 through August 31. YouTube rolled out custom thumbnails for Shorts (July 24 — one of the most-requested creator features ever), AI-powered thumbnail generation in Ask Studio, and introduced an "inauthentic content" monetization ban (July 16) covering generic/template videos and AI persona advice content. MCP Tunnels entered public beta — outbound-only encrypted connections for private-network data access without inbound firewall rules, with Cloudflare/Daytona/Modal/Vercel as sandbox providers. Statewave (Apache-2.0) launched a production-ready MCP server for persistent cross-session agent memory on self-hosted Postgres+pgvector — a major gap in the robot stack now filled for free. OpenAI Assistants API shuts down **August 26, 2026 — 26 days from today**: migrate to Responses API or all `/v1/assistants`, `/v1/threads`, and `/v1/runs` calls return errors. Activepieces confirmed as the best new free automation alternative (10 flows, unlimited runs, open-source). YouTube Shorts clickable Channel Page links launch August 23.

---

## Week of 2026-07-24 — Recon Summary

**Major finds this week:** Webflow MCP 2.0 launched July 21 — governance, design-system enforcement, and analytics for AI-driven web management (free on all plans, remote OAuth). GitHub MCP Server updated July 23 to support the new stateless 2026-07-28 spec ahead of release. Sprinklr MCP (Beta, July 15) — first major social listening platform with an official MCP. Previously undocumented MCPs confirmed live: Kit/ConvertKit (official, 13 tools), Monday.com (official, full workspace CRM + PM), Asana V2 (GA, 42 tools — V1 shut down May 11), Pinterest (official, June 17 — live ad analytics), Zoom (expanded May 2026 — 10 enterprise app integrations), Mailchimp (official transactional + community full marketing API), Snowflake (native Cortex Analyst/Search/SQL). Instagram engagement quantification confirmed: DM share ≈ 15 likes, save ≈ 10 likes — DM-share engineering is now the #1 Instagram growth lever. Instagram posts now tracked in Google Search Console (July 7) — IG is officially an SEO channel. LinkedIn Suggested Posts / Topic-Focused Feeds entering wider rollout — quality posts distributed to interested users for months. X replies now weighted 27x over likes (upgraded from 13.5x). DeepSeek `deepseek-chat` and `deepseek-reasoner` aliases retired today at 15:59 UTC — migrate to `deepseek-v4-flash` or `deepseek-v4-pro` immediately. Cloudflare Workers Cache (July 6) — cached automation endpoints cost zero CPU time, free in Workers free tier.

---

## Week of 2026-07-17 — Recon Summary

**Major finds this week:** Meta Muse Spark 1.1 API launched July 9 — Meta's first paid AI model, priced aggressively at $1.25/$4.25 per M tokens, free tier $20 credits + 60 req/min. Supabase shipped an official Remote MCP server (OAuth login flow, no more PAT required, 20+ tools). Linear launched an official hosted MCP server. Gumloop MCP Hub now provides 100+ fully hosted MCP servers (Salesforce, HubSpot, GitHub, Jira, Slack, etc.) on free tier. Discord integration MCP servers confirmed (community-built, multiple implementations). X algorithm major update July 13: Nikita Bier confirmed mutual-follower priority weighting — replies/posts from mutuals now rank above strangers, 2x increase in original posts/replies observed. YouTube formally confirmed viewer satisfaction (surveys + repeats + shares) as primary signal, replacing raw watch time. Instagram expanded carousels to 20 frames, confirmed 3-min Reel recommendation ceiling (can upload up to 20 min but algo stops pushing to non-followers after 3 min).

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
| **Snowflake** ⭐ NEW (OFFICIAL) | Three native tools: Cortex Analyst (natural-language to SQL over your data), Cortex Search (unstructured/semantic content search), SYSTEM_EXECUTE_SQL (direct SQL with optional read-only flag). RBAC and data masking inherited from your existing Snowflake permissions. Zero infrastructure — runs inside your Snowflake account. | Data warehouse robot — NL queries over business data, semantic search across unstructured docs, automated reporting from Snowflake tables | No install — enable in Snowflake Cortex settings. GA November 4, 2025. |
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
| **Kit (ConvertKit)** ⭐ NEW (OFFICIAL) | 13 tools — full Kit V4 API: analytics, subscribers, forms, sequences, broadcasts, commerce, tags, segments, bulk operations. Auth handled automatically. Separate Kit Developer Docs MCP for building integrations. | Email subscriber management robot, list segmentation, broadcast automation, revenue tracking from email sales | Remote OAuth: `developers.kit.com/mcp` (all Kit plans) |

### Email, Outreach & Messaging
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Postmark (by ActiveCampaign)** ⭐ NEW (OFFICIAL) | 24 tools: single + batch email sending (up to 500/call), template CRUD + validation, message search, delivery diagnostics (diagnoseDelivery tool), bounce management, suppression lists, webhooks, server info. Open source MIT. | Transactional email robot — send AI-drafted emails, diagnose deliverability, manage templates, bulk sends | Clone: `github.com/ActiveCampaign/postmark-mcp` (requires Postmark API key) |
| **Klaviyo** | Email marketing, campaigns, segments, profiles | Email robots, list management, campaign automation | Native |
| **Mailchimp** ⭐ NEW | Official: transactional email (Mandrill) — `mandrillapp.com/mcp`. Community full-stack: 112 tools covering campaigns, audiences, reports, segments, automations, e-commerce, with dry-run safety mode. | Email campaign robot, transactional email, audience segmentation, e-commerce email automation | Official: `https://mandrillapp.com/mcp` (API key required); Community full-stack: `github.com/damientilman/mailchimp-mcp-server` |
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
| **Webflow** ⭐ NEW (OFFICIAL V2) | Design, build, and manage Webflow sites via AI — v2 adds governance layer: branch-based editing, role/permission enforcement (per-site/page/locale/CMS collection), AI attribution in activity log, reusable Agent Instructions for brand/voice/legal constraints, performance analytics (traffic trends, top pages, engagement). Design system (typography, colors, spacing tokens, component variants) exposed as structured data agents can query and obey. | Web publishing robot, CMS content management, landing page creation and iteration, on-brand design automation, site performance analytics | Remote OAuth: `https://mcp.webflow.com/sse` (all Webflow plans, free included); open source: `github.com/webflow/mcp-server` — Launched July 21, 2026 |

### Social Media
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Meta Ads (Official)** ⭐ NEW (OFFICIAL) | 29 tools — campaign creation/management, ad groups, creatives, audience targeting, catalog management, performance analytics, insights. Standard Business OAuth. Open beta as of Apr 29, 2026. Works across Facebook + Instagram Ads Manager. | Full Meta Ads robot — create campaigns, manage budgets, monitor ROAS, generate creative variations, audience management | Remote: Meta Ads Connectors in Business Suite (no developer app needed); or community: `github.com/pipeboard-co/meta-ads-mcp` |
| **Meta Comprehensive (Community)** ⭐ NEW | 200+ tools: Facebook Pages, Instagram, Threads, Ads Manager, Commerce, Conversions API, Custom Audiences, Insights, Ad Library | Full Meta platform robot — organic + paid, organic posting on Pages/IG/Threads plus ad ops in one server | `github.com/oliverames/meta-mcp-server` (community, MIT) |
| **X (Twitter)** ⭐ NEW (OFFICIAL) | 200+ endpoints — search, timelines, user lookups, DMs, lists (read-heavy; write endpoints NOT exposed) | Social listening, trend monitoring, audience research. Note: cannot post via this MCP | Remote OAuth: `https://developer.x.com/en/products/x-api/mcp` (Launched June 30, 2026) |
| **TikTok Ads** ⭐ NEW | Campaign management, ad groups, creatives, audience targeting, performance analytics | TikTok ad campaign robot, performance monitoring, creative management | `pip install tiktok-ads-mcp` (requires TikTok Business API access) |
| **Reddit** ⭐ NEW | Read subreddits, posts, comments, search, user profiles, hot/new/top feeds | Community monitoring, trend detection, social listening robot | `npx reddit-mcp-server` (requires Reddit API credentials) |
| **Ayrshare** ⭐ NEW | 75+ tools across 13 platforms (X, FB, IG, LI, TikTok, YouTube, Pinterest, Reddit, Threads, Bluesky, more) | Multi-platform posting robot, analytics, comment management — one server for all social | `npx -y @ayrshare/mcp-server` (requires Ayrshare API key) |
| **Pinterest** ⭐ NEW (OFFICIAL) | Read-only: live campaign analytics, ad performance data, keyword insights — mirrors what's available in the Pinterest Ads Manager API. Internal at Pinterest: 66,000 invocations/month, 7,000+ hours saved/month. External MCP launched alongside Microsoft Advertising MCP on June 17, 2026. | Pinterest ad analytics robot, keyword research, campaign performance monitoring | Community server: `github.com/collactivelabs/pinterest-mcp-server` (requires Pinterest API credentials) — Launched June 17, 2026 |
| **Sprinklr** ⭐ NEW (BETA) | Social listening, customer experience (CX) intelligence, brand mentions, competitor monitoring. Part of Summer '26 release which adds video intelligence (ViralMoment), generative AI search tracking (LLM Insights), and creator/performance data (CreatorIQ). Compatible with Claude, Microsoft Copilot, and ChatGPT. | Social listening robot, brand monitoring, competitor tracking, CX analytics | Beta — contact Sprinklr. Launched July 15, 2026 |
| **Discord (Community)** ⭐ NEW | Send/read messages, manage channels, forum operations, reactions, webhook management — multiple community implementations. Read and send messages, manage channels and forums, handle reactions, interact with webhooks directly. | Community management robot, Discord notification bot, server monitoring, channel-based alerts | Multiple options: `github.com/v-3/discordmcp`; `github.com/SaseQ/discord-mcp`; `github.com/IQAIcom/mcp-discord` (requires Discord bot token) |

### Ecommerce
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Shopify** ⭐ NEW (SUITE of 4) | **Storefront**: product catalog, cart, policies; **Customer Accounts**: orders, returns, tracking; **Admin**: full store ops; **Dev**: GraphQL schema | Full Shopify automation — catalog management, order robots, customer service, inventory | Remote hosted (add Shopify MCP endpoint); Community: `npx -y @geli2001/shopify-mcp` (MIT, April 2026) |

### Project Management
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Linear** ⭐ NEW (OFFICIAL) | Issues, projects, teams, cycles, milestones, roadmaps, documents — full Linear GraphQL API. Create/update issues, change status, assign, comment. | Project management robot, sprint tracking, issue creation from Claude conversations, release notes | Official remote endpoint (PulseMCP); or `npx add-mcp @tacticlaunch/mcp-linear --env LINEAR_API_TOKEN=YOUR_TOKEN` |
| **ClickUp** ⭐ NEW (OFFICIAL, PUBLIC BETA) | Task management with assignees/priorities/due dates, time tracking (start/stop timers, log entries), Docs read/write, comment summarization, executive report generation. Available on all plans. Rate limits: 50 calls/24h (Free), 300 calls/24h (Unlimited+); unlimited with Everything AI add-on. | Project management robot, release notes, status reports, task creation from AI conversations, time tracking | In-app: ClickUp Settings → Integrations → MCP; or `claude mcp add clickup` pointing to ClickUp's hosted endpoint |
| **Atlassian (Jira + Confluence + Bitbucket)** ⭐ NEW | Rovo search across Jira/Confluence, create/update issues and epics, Confluence pages, semantic search | Project management robot, issue tracking, documentation automation | Remote OAuth: `https://mcp.atlassian.com` (GA Feb 4, 2026; free for all Atlassian Cloud customers) |
| **Monday.com** ⭐ NEW (OFFICIAL) | Full workspace access — CRM, project management, operations data. Plug-and-play. All boards, items, sub-items, columns, automations, dashboards. Claude, ChatGPT, and Microsoft Copilot compatible. | Project + CRM robot — manage tasks, boards, deals, contacts from AI; automate status updates and notifications | `npm install @mondaydotcomorg/monday-api-mcp`; Docs: `monday.com/w/mcp` (free on all Monday.com plans) |
| **Asana** ⭐ NEW (OFFICIAL V2) | 42 tools — task and project management, workload analysis, search, team/workspace management. V2 uses OAuth 2.0 + Streamable HTTP; respects existing Asana access controls. V1 (SSE) shut down May 11, 2026 — must use V2. Two bulk tools added April 13: `create_tasks` and `update_tasks` for dependency and section management. | Project management robot, sprint tracking, task creation from AI conversations, workload analysis, automated status updates | Remote: `https://mcp.asana.com/v2/mcp` (OAuth, all Asana plans) — GA February 4, 2026 |
| **Zoom** ⭐ NEW (OFFICIAL, EXPANDED) | Meeting summaries, transcripts, recordings, scheduling. May 2026 expansion added agentic search across 10 enterprise platforms: Salesforce accounts, Workday employee/time-off records, ServiceNow tickets/incidents, plus 7 more connected services. Surfaces cross-system context during meetings. | Meeting intelligence robot, meeting summary distribution, cross-platform data retrieval during conversations | Remote OAuth (Zoom Developer Portal); Community: `github.com/echelon-ai-labs/zoom-mcp` — Expanded May 2026 |

### Infrastructure & Deployment
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **DigitalOcean** | App deployment, hosting, management | Deploy dashboards, landing pages, tools | Native |
| **Stitch** | UI design system generation | Dashboard and tool UI creation | Native |
| **Supabase** ⭐ NEW (OFFICIAL REMOTE) | 20+ tools: managed Postgres, schema design, SQL queries, migrations, Edge Functions, Auth, Storage, Realtime DB, branching, log retrieval, docs search. No PAT needed — OAuth login flow built in. | Full backend robot — spin up DB, design tables, query data, deploy functions, manage auth, debug with logs | Remote OAuth (auto-redirects on setup): `npx @supabase/mcp`; or configure in Cursor/Windsurf/Claude Code settings. Launched GA 2026. |
| **Cloudflare** ⭐ NEW | 2,500+ endpoints — DNS, Workers, R2 storage, Pages, Zero Trust, KV, D1, WAF | Full infrastructure automation, edge function deployment, CDN management | Remote OAuth: `https://mcp.cloudflare.com`; or `npx -y @cloudflare/mcp-server` |
| **Vercel** ⭐ NEW | Projects, deployment status, env vars, domains, logs, team settings | Deployment robot, env var management, monitoring | `claude mcp add --transport http vercel https://mcp.vercel.com` (OAuth, no local install) |
| **AWS** ⭐ NEW (OFFICIAL) | Full AWS API — CloudFormation, ECS, S3, Lambda, IAM, CDK, docs, cost management | Cloud infrastructure automation, serverless deployment, cost monitoring | `pip install awslabs.core-mcp-server` (GA May 2026; uvx recommended) |
| **Firebase** ⭐ NEW | Firestore, Auth, Storage, Functions, Hosting, Realtime DB — full read/write | Database robots, user management, serverless automation | `npx -y firebase-tools@latest mcp` (built into firebase-tools CLI) |
| **Kubernetes / OpenShift** ⭐ NEW (Aug 12, 2026) | Full CRUD on K8s resources (pods, deployments, services); log/metric/event queries; Helm ops; OpenShift support. Uses existing kubeconfig. | Cluster management robot, auto-scaling automation, log analysis, cost monitoring for self-hosted growth robot infra | `npx @kubernetes/mcp-server` (set `KUBECONFIG`); `github.com/containers/kubernetes-mcp-server` (Apache-2.0, v0.0.65) |

### Automation & Workflow
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **n8n** ⭐ NEW | Trigger existing workflows, build/edit workflows (v2.13+), all n8n nodes accessible | AI-triggered automation robot — kick off any n8n workflow from Claude | Built-in to n8n — enable in settings, point MCP client at n8n instance URL |
| **Gumloop MCP Hub** ⭐ NEW | 100+ fully hosted MCP servers for Salesforce, HubSpot, GitHub, Jira, Slack, Loops, and more. Free plan includes all hosted servers. Pro ($37/mo) adds custom MCP server proxying. No-code AI agent builder + MCP access in one platform. | AI agent orchestration robot, connect agents to 100+ apps without managing server infra; free tier is generous for small-scale growth robots | `gumloop.com/mcp` — OAuth connection, no local install. Free plan: 5K credits/month, 1 active trigger, 5 concurrent agent runs |

### Newsletter Publishing
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Substack Publisher MCP** ⭐ NEW (COMMUNITY) | Query Substack Publisher API: post analytics, subscriber counts, publication data — read-focused | Newsletter analytics robot — pull subscriber growth, post performance, and revenue data from Claude | `github.com/dkships/substack-publisher-mcp` (requires Substack Publisher API key) |
| **Substack Automation MCP** ⭐ NEW (COMMUNITY) | Create posts, manage drafts, publish Notes, interact with Substack's API | Newsletter automation robot — draft generation, Notes scheduling, content management | `github.com/marcomoauro/substack-mcp`; or `github.com/conorbronsdon/substack-mcp` (draft-only safety design — cannot publish long-form, only Notes) |
| **Postcli Substack MCP** ⭐ NEW (COMMUNITY) | Full content management — posts, Notes, comments, profiles, social interactions | Substack social engagement robot, content management, cross-post scheduling | `pulsemcp.com/servers/postcli-substack` (launched March 2026) |

### Knowledge & Memory
| MCP | What It Does | Growth Robot Use | Install |
|-----|-------------|-----------------|---------|
| **Statewave** ⭐ NEW (APACHE-2.0) | Open-source memory runtime for AI agents — durable, structured context with provenance across sessions. 5 tools: store memory, retrieve context, compile memory bundles. Reproducible context bundles instead of query-time retrieval. Self-hosted on Postgres + pgvector. Python + TypeScript SDKs. Vendor-neutral (no IDE, model provider, or hosted dependency assumptions). | Persistent agent memory robot — prevents growth robots from "forgetting" between sessions; build long-running automation agents that accumulate knowledge over time; multi-agent workflows with shared context stores | `npm install @statewavedev/mcp-server` (npm); or Docker: `statewavedev/statewave-mcp-server`; GitHub: `github.com/smaramwbc/statewave` — Apache-2.0, self-hosted, July 2026 |

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

## MCP Protocol — 2026-07-28 Spec (OFFICIALLY SHIPPED July 28, 2026)

> **Live as of July 28, 2026.** Biggest spec revision since MCP launched. The ecosystem has crossed 10,000+ production servers and 400M monthly SDK downloads (4x growth in 2026). Claude now supports the new spec across all products. The RC became the official spec on July 28 after a 10-week validation window. Affects how servers are deployed and what capabilities they can expose.

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

## Critical API Deprecations & Shutdowns (Week of 2026-08-14)

> **EMERGENCY — Act within days:**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **Anthropic Workbench (Legacy)** | Legacy Workbench at `platform.claude.com/workbench` permanently shut down — all saved prompts, prompt versions, and evals inside it become inaccessible. Also retiring: `/v1/experimental/generate_prompt`, `/v1/experimental/improve_prompt`, `/v1/experimental/templatize_prompt` (all experimental prompt tool APIs). The new Workbench is a simpler stateless playground; it does not import saved legacy data. | **Aug 17, 2026 (3 DAYS)** | Export all saved prompts and evals from legacy Workbench TODAY. Stop calling the three experimental prompt API endpoints — they error after Aug 17. |
| **Google Merchant Content API for Shopping** | Already logged last week — still 4 days away and actively failing for anyone who hasn't migrated. Silent pricing trap: Merchant API v1 uses different `price`/`sale_price` field names. | **Aug 18, 2026 (4 DAYS)** | Migrate to Merchant API v1 NOW. Test price fields before flip or live products misprice silently. |
| **OpenAI Assistants API** | Already logged — 12 days to complete shutdown of `/v1/assistants`, `/v1/threads`, `/v1/runs` | **Aug 26, 2026 (12 days)** | Migrate to Responses API. Azure users have until Feb 2027. No automated thread migration tool — rebuild manually. |

> **Pricing change confirmed permanent (act to lock in):**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **Claude Sonnet 5** | Introductory pricing of $2 input / $10 output per MTok is NOW PERMANENT (Anthropic confirmed Aug 11, 2026). The planned September 1 step-up to $3/$15 was cancelled. **BUT:** Sonnet 5 uses a new tokenizer that produces ~30% more tokens from the same input text vs. prior models — effective cost per request may be higher than pricing alone suggests. | **Permanent as of Aug 11** | Re-run your token benchmarks on Sonnet 5 with real prompts (don't just compare per-MTok price). The $2/$10 rate is locked but the per-request cost depends on how the tokenizer handles your specific content. |

---

## New Tools & Infrastructure (Week of 2026-08-14)

### Kubernetes MCP Server — AI-Driven Cluster Management (Updated August 12, 2026)

Official Red Hat/containers project for managing Kubernetes and OpenShift clusters via MCP. Production-ready, updated August 12, 2026. v0.0.65 is the latest release (July 14).

| Detail | Value |
|--------|-------|
| **Source** | `github.com/containers/kubernetes-mcp-server` (Apache-2.0) |
| **What it connects to** | Any Kubernetes cluster + OpenShift — uses your existing kubeconfig credentials |
| **What it exposes** | Full CRUD on K8s resources (pods, deployments, services, etc.); query logs, metrics, and events; automate scaling, monitoring, troubleshooting; Helm operations |
| **Also** | Separate companion: `github.com/openshift/openshift-mcp-server` (OpenShift-specific) |
| **Install** | `npx @kubernetes/mcp-server` or binary from releases page; configure with `KUBECONFIG` env var |
| **Growth robot potential** | MEDIUM-HIGH for infrastructure clients — AI-driven cluster management, auto-scaling robots, log analysis, cost optimization; not directly a growth tool but enables self-hosted growth robot infrastructure |

---

## Critical API Deprecations & Shutdowns (Week of 2026-08-07)

> **EMERGENCY — Act within days:**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **Google Merchant Content API for Shopping** | Complete shutdown — every programmatic call to the Content API starts failing at 00:01 UTC. Only manual file/CSV uploads via Merchant Center are unaffected. Cascade: product sync stops, new products don't appear in Shopping, edits don't update, inventory sync stops. Silent mispricing trap: the new Merchant API v1 uses different price/sale_price field names — migration without testing causes live products to show wrong prices. | **Aug 18, 2026 (11 days)** | Migrate to Google Merchant API v1 NOW. Migration guide: `brightbid.com/blog/google-merchant-api-migration-2026/`. Test price fields before going live. |
| **OpenAI Assistants API** | Already logged — complete shutdown of `/v1/assistants`, `/v1/threads`, `/v1/runs` | **Aug 26, 2026 (19 days)** | Migrate to Responses API + Conversations API. Azure users have until Feb 2027. |

---

## MCP Ecosystem Milestone (Week of 2026-08-07)

**22,311 MCP servers** now indexed on PulseMCP as of July 16, 2026. Governance of the MCP specification has been transferred to the **Linux Foundation's AAIF (AI Alliance Infrastructure Foundation)** — the same body that governs ONNX and OpenXLA. Implications:
- MCP is now formally vendor-neutral infrastructure, not an Anthropic-controlled protocol
- Enterprise procurement teams can now justify MCP adoption under neutral open-source governance
- Spec changes will follow Linux Foundation RFC process — slower but more stable than Anthropic's direct ship model
- All Tier 1 SDKs (TypeScript, Python, Go, C#) speak the 2026-07-28 stateless spec

**Growth robot implication:** Build MCP-native robots with confidence — the spec is now as stable and vendor-neutral as HTTP. No single provider can pull the rug.

---

## Critical API Deprecations & Shutdowns (Week of 2026-07-31)

> **URGENT — Act within days:**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **OpenAI Assistants API** | Complete API shutdown — `/v1/assistants`, `/v1/threads`, `/v1/runs` all return errors after deadline. No automated migration tool — manual backfill of Threads → Conversations required. Azure OpenAI has until Feb 2027. | **Aug 26, 2026** (26 days away) | Migrate all OpenAI Assistants bots to the Responses API + Conversations API NOW — not next week. See `developers.openai.com/api/docs/assistants/migration` |

> **Pricing changes (act by August 31):**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **Claude Sonnet 5** | Introductory pricing $2/$10 per MTok (input/output) — will rise after August 31 | **Aug 31, 2026** (pricing window) | Lock in Sonnet 5 for any robots launched before September; budget accordingly |

---

## New Tools & Infrastructure (Week of 2026-07-31)

### Claude Opus 5 — New Flagship API Model (July 24, 2026)

Anthropic's latest Opus-tier model: near-Fable-5 intelligence at half the cost. Surpasses all other non-Fable models on Frontier-Bench v0.1 and CursorBench 3.2.

| Detail | Value |
|--------|-------|
| **Release date** | July 24, 2026 |
| **Context window** | 1M tokens input, 128K output |
| **Pricing (input/output)** | $5/$25 per MTok standard; $10/$50 fast mode; $2.50/$12.50 batch |
| **Adaptive thinking** | On by default |
| **Knowledge cutoff** | May 2026 |
| **Availability** | Anthropic API, Amazon Bedrock, Google Cloud, Microsoft Foundry |
| **vs Fable 5** | Within 0.5% on CursorBench at half the cost per task |
| **Growth robot potential** | HIGH — use Opus 5 for complex agentic robots where Sonnet doesn't cut it but Fable 5 is overkill; batch API at $2.50/$12.50 makes it cost-competitive for bulk operations |

**Current Claude pricing hierarchy (July 2026):** Fable 5 ($10/$50) → Opus 5 ($5/$25) → Sonnet 5 ($3/$15, intro $2/$10 through Aug 31) → Haiku 4.5 ($1/$5)

---

### MCP Tunnels — Private Network Access Without Firewall Rules (Public Beta)

Announced at Code with Claude London (May 19, 2026). MCP Tunnels open an outbound-only encrypted connection from a private network to the MCP host. Agents reach customer/internal data without any inbound firewall rule changes.

| Detail | Value |
|--------|-------|
| **Status** | Public beta (self-hosted sandboxes) |
| **Sandbox providers** | Cloudflare, Daytona, Modal, Vercel |
| **Use case** | Connect growth robots to private databases, internal CRMs, on-prem tools — without exposing them to the internet |
| **Growth robot potential** | HIGH for enterprise clients; allows full CRM/database robot access on customer infrastructure |
| **Source** | `claude.com/blog/bringing-mcp-2026-07-28-to-claude` |

---

### Statewave — Persistent Agent Memory (Apache-2.0, Free)

Open-source memory runtime for AI agents. Prevents robots from forgetting context between sessions. Self-hosted on Postgres + pgvector. Reproducible provenance-tagged context bundles. 5 MCP tools exposed. Launched on Product Hunt July 28, 2026.

See **Knowledge & Memory** table above for full entry.

---

### Activepieces — Best New Free Automation Alternative (July 2026)

Open-source automation platform with the most generous free cloud tier in July 2026.

| Detail | Value |
|--------|-------|
| **Free tier** | 10 flows, unlimited runs, no credit card |
| **Open source** | Yes (self-hostable) |
| **vs Make** | Make: 1,000 ops/month cap; Activepieces: unlimited runs on free |
| **vs n8n** | n8n requires self-hosting for unlimited; Activepieces free cloud tier |
| **Interface** | Clean drag-and-drop, similar to Make |
| **Growth robot potential** | MEDIUM — best cloud free tier for small automation robots; good fallback when Make quota runs out |
| **Install** | `activepieces.com` or self-host |

---

## Critical API Deprecations & Shutdowns (Week of 2026-07-24)

> **URGENT — Act today or by month-end:**

| API / Service | What Changed | Effective Date | Action Required |
|---|---|---|---|
| **DeepSeek `deepseek-chat` + `deepseek-reasoner`** | Legacy model name aliases retired — calls return errors after cutoff | **Jul 24, 2026 at 15:59 UTC** | Migrate to `deepseek-v4-flash` (non-thinking) or `deepseek-v4-pro` (higher-tier). Same base URL, same API key, same request structure. Also: new Anthropic-format endpoint at `https://api.deepseek.com/anthropic` for Claude Code clients |
| **Zapier — Pipedrive V1 API triggers/actions/searches** | Replaced by V2 versions; V1 deprecated and removed from Zapier | **Jul 31, 2026** | Update any Zapier/Pipedrive Zaps to V2 versions before month end |
| **OpenAI legacy audio/realtime/transcription snapshots** | Deprecated July 20; full removal from API January 20, 2027 | **Jan 20, 2027** (removal) | Audit any OpenAI audio/realtime/transcription automation; migrate to current model IDs |
| **Cloudflare Gateway Audit SSH Action** | Network policy action fully removed | **Jul 15, 2026** (done) | Remove from any Cloudflare Zero Trust network policies |
| **ProductBoard API v1** | Sunset — v2 (launched April 9, 2026) is now the only supported version | **Jul 8, 2026** (done) | Migrate to ProductBoard API v2 |

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

## New Free Tools & APIs — Week of 2026-07-24

### Cloudflare Workers Cache — Zero-CPU Cached Endpoints (July 6, 2026)

A regionally tiered cache for Cloudflare Worker entrypoints. Configured with standard `Cache-Control` headers and one line in `wrangler.toml`. When a cached response exists, the Worker does **not run** and you are **not billed CPU time**.

| Detail | Value |
|--------|-------|
| **Free tier** | Included in Workers free tier (100,000 requests/day) |
| **Configuration** | `cache_rules` in `wrangler.toml` + standard `Cache-Control` headers |
| **New companion tools** | Wrangler Flagship CLI (feature flags without redeployment); Temporary Accounts API (deploy Workers before user sign-in, for SaaS onboarding) |
| **Growth robot potential** | HIGH — cache heavy-read automation endpoints to reduce CPU cost to zero |
| **Source** | `blog.cloudflare.com/workers-cache/` |

---

### Ollama — $65M Series B (July 9, 2026)

Free open-source platform for running LLMs locally — Llama 4, Mistral, Qwen, DeepSeek-R1, CodeLlama, and 200+ others. No API key, no cloud, no rate limits on local inference.

| Detail | Value |
|--------|-------|
| **Free tier** | 100% free for local use (unlimited). Cloud execution available for larger models |
| **Scale** | 8.9 million monthly developers, 67,000 integrations, 85% of Fortune 500 |
| **Why it matters** | Cheapest inference per token available for any repeatable automation task |
| **Growth robot potential** | HIGH — zero-cost local inference for content generation, classification, and embedding pipelines |
| **Install** | `ollama.ai` — one-command install on Mac, Windows, Linux |

---

### Resend Email API — Rebuilt Free Tier Email Tool

Developer-first transactional email API with a fully rebuilt no-code email editor (100% rollout as of July 2026). Best free tier in transactional email for automation.

| Detail | Value |
|--------|-------|
| **Free tier** | 3,000 emails/month, 1 domain, 100 emails/day (no credit card) |
| **What's new** | Rebuilt no-code email editor — new layout, HTML formatter (Prettier), drag-and-drop block reordering. API batch email latency improvements |
| **Growth robot potential** | HIGH — free transactional email at reasonable volume for small growth robots |
| **Install** | `resend.com` + API key |

---

### GitHub Copilot CLI in Actions — No PAT Required

GitHub Copilot CLI now runs inside GitHub Actions using the built-in `GITHUB_TOKEN` — no Personal Access Token required.

| Detail | Value |
|--------|-------|
| **Free tier** | GitHub Actions free tier (unlimited on public repos; 2,000 min/month on private) |
| **What this unlocks** | AI-augmented CI/CD pipelines without managing PATs — lower friction for agentic automation inside repos |
| **Growth robot potential** | HIGH for technical automation pipelines. AI can now comment, create issues, and modify code within Actions at no extra cost |
| **Source** | `github.blog/changelog/month/07-2026/` |

---

## New Free Tools & APIs — Week of 2026-07-17

### Meta Muse Spark 1.1 — New AI API with Free Credits

**Launched:** July 9, 2026. Meta's first paid, closed-weights AI model. Multimodal reasoning model built for long, tool-heavy agentic tasks — planning and orchestration across apps and services.

| Detail | Value |
|--------|-------|
| **Free tier** | $20 free credits + 60 requests/min, 2M tokens/min |
| **Input price** | $1.25/M tokens (cached: $0.15/M — extremely cheap for agentic pipelines where system prompts repeat) |
| **Output price** | $4.25/M tokens |
| **Context window** | Not disclosed in search |
| **Availability** | US-based developers only (public preview) |
| **SDK** | Full SDK + CLI available at launch |
| **Paid tier** | 3,000 req/min, 4M tokens/min |

**Growth Robot Potential:** High-volume agentic pipelines where tool orchestration matters more than single-step quality. The $0.15/M cached input token price makes it the cheapest option for robots with large, repetitive system prompts. Benchmark against GPT-4.1 and Claude Sonnet before committing — pricing is ~25% of flagship OpenAI/Anthropic rates.

**Install:** `meta-ai` SDK (see `developer.meta.com/ai/resources/blog/build-with-muse-spark/`)

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
