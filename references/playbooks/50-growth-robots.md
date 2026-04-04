# 50 Growth Robot Blueprints

**Purpose:** Pre-built robot ideas the CGA can recommend and adapt to any business. Each is a literal technical automation — code, APIs, webhooks, scheduled tasks — that forms a self-feeding loop.

**Three-question test (all must be YES):**
1. Can you turn it off? (It's deployed software)
2. Running without humans? (Autonomous)
3. Each cycle's output feeds the next input? (Self-feeding)

**Categories:** Content Growth (1-18), Email List Growth (19-34), Lead Generation (35-50)

---

## CONTENT GROWTH ROBOTS

### Robot 1: The Clipping Multiplier
**Loop:** Long-form video → AI clips into 20-30 shorts → posted across 5-10 accounts on IG/TikTok/Shorts → viewers follow main channel → main channel creates more long-form → more clips
**Parts:** Product (content), AI Agents (clipping), APIs (scheduling + posting), Users (viewers)
**Hat:** `[GREY]` — multiple accounts may bend TOS
**Build:** AI transcription → clip identification → auto-edit with captions → schedule via Buffer/Later → track which clips drive main-channel follows

### Robot 2: The Comment-to-Content Engine
**Loop:** Monitor competitor/industry posts via API → AI generates insightful comments → post comments with profile linking to content → profile visitors become followers → more content → more comments to make
**Parts:** APIs (social listening), AI Agents (comment generation), Users (profile visitors), Product (content)
**Hat:** `[GREY]` — automation of engagement
**Build:** Social listening API → GPT comment generator → posting scheduler → follower tracking

### Robot 3: The Trend Rider
**Loop:** Monitor trending sounds/topics via API → AI generates content matching trend within minutes → post before trend peaks → algorithm boosts trending content → more followers → more content capacity
**Parts:** APIs (trend monitoring), AI Agents (content generation), Applications (posting tools), Product (content)
**Hat:** `[WHITE]`
**Build:** TikTok/IG trend API → content template system → AI adaptation → auto-post → performance tracking

### Robot 4: The Quote Extraction Machine
**Loop:** Scrape podcast/video transcripts → AI extracts quotable moments → auto-generate branded quote cards → post with attribution + link → creators reshare (free distribution) → their audience discovers you → more content to quote
**Parts:** APIs (transcription), AI Agents (extraction + design), Users (original creators who reshare), Applications (Canva API)
**Hat:** `[WHITE]` — attribution makes it ethical
**Build:** Whisper transcription → GPT quote extraction → Canva API design → schedule posts → track reshares

### Robot 5: The UGC Amplifier
**Loop:** Customers mention your brand → automation detects mention → AI generates thank-you + reshare → reshared content reaches customer's audience → new customers mention brand → loop
**Parts:** APIs (social monitoring), AI Agents (response generation), Users (customers), Product (your brand)
**Hat:** `[WHITE]`
**Build:** Brand mention monitoring → auto-reshare workflow → personalized thank-you DM → track new mentions from reshare audience

### Robot 6: The Content Repurposer
**Loop:** Blog post published → AI converts to: Twitter thread + LinkedIn carousel + IG carousel + email newsletter + YouTube script → each format reaches different audience → traffic back to blog → more blog posts
**Parts:** AI Agents (format conversion), APIs (publishing), Product (blog), Applications (design tools)
**Hat:** `[WHITE]`
**Build:** RSS feed trigger → AI reformatter → platform-specific publishing APIs → UTM tracking → analytics

### Robot 7: The SEO Content Factory
**Loop:** Keyword research API finds low-competition keywords → AI writes optimized article → published to blog → Google indexes → organic traffic → traffic data reveals new keyword opportunities → more articles
**Parts:** APIs (keyword research, Google Search Console), AI Agents (writing), Product (blog), Applications (CMS)
**Hat:** `[WHITE]`
**Build:** Ahrefs/SEMrush API → GPT article generation → WordPress API publish → GSC monitoring → new keyword identification → loop

### Robot 8: The Collaboration Snowball
**Loop:** Identify accounts in your niche with similar follower count → auto-DM collaboration pitch → create collab post/video → both audiences see it → both accounts grow → qualify for bigger collaborations → bigger audiences
**Parts:** APIs (account discovery), AI Agents (pitch writing), Users (collaborators), Product (content)
**Hat:** `[GREY]` — automated DMs may violate TOS
**Build:** Social API follower analysis → AI pitch generator → DM automation → collab content tracker → growth measurement

### Robot 9: The Evergreen Recycler
**Loop:** Track best-performing content → after 90 days, AI rewrites/remixes top performers → repost → algorithm treats as new content → new audience sees it → new followers → more content to recycle
**Parts:** APIs (analytics), AI Agents (rewriting), Applications (scheduling), Product (content library)
**Hat:** `[WHITE]` — with genuine rewrites. `[GREY]` — with metadata tricks for "uniqueness"
**Build:** Analytics API → identify top 10% performers → AI rewrite with new hook/angle → schedule repost → compare performance

### Robot 10: The Podcast Guest Engine
**Loop:** Scrape podcast directories for shows in your niche → AI writes personalized pitch emails → book appearances → each appearance links back to your content → new audience discovers you → some become podcast hosts themselves → more shows to pitch
**Parts:** APIs (podcast directories), AI Agents (pitch writing), Applications (email), Users (podcast hosts)
**Hat:** `[WHITE]`
**Build:** Listen Notes API → AI pitch personalization → email automation → appearance tracking → backlink monitoring

### Robot 11: The Reply Guy Bot
**Loop:** Monitor industry thought leaders' posts → within 60 seconds of posting, add valuable first comment → early comments get most visibility → viewers click your profile → followers grow → more authority → comments get even more visibility
**Parts:** APIs (post monitoring), AI Agents (comment generation), Applications (social platforms)
**Hat:** `[GREY]` — automated engagement
**Build:** Twitter/LinkedIn API monitoring → notification trigger → AI comment generator → auto-post → profile click tracking

### Robot 12: The Newsletter Cross-Pollinator
**Loop:** Write newsletter → include "share with a friend" incentive (unlock bonus content) → subscribers share → new subscribers join → they share with THEIR friends → exponential list growth → more content to share
**Parts:** Product (newsletter), APIs (email platform), Users (subscribers who share), AI Agents (bonus content generation)
**Hat:** `[WHITE]`
**Build:** Beehiiv/ConvertKit referral program → tiered rewards → automated bonus content delivery → share tracking

### Robot 13: The Metadata Uniqueness Engine
**Loop:** Take top-performing video → AI modifies: crop ratio, color grading, speed (1.01x), audio pitch, caption style, intro frame → platform sees "unique" content → distributes again → more views → identify next video to recycle
**Parts:** AI Agents (video modification), APIs (posting), Applications (FFmpeg), Product (content library)
**Hat:** `[GREY]` to `[BLACK]` — explicitly gaming uniqueness detection
**Build:** FFmpeg automation → random parameter variation → batch upload → performance tracking → identify winners for next cycle

### Robot 14: The Thread-to-Carousel Pipeline
**Loop:** Write Twitter thread → AI auto-converts to LinkedIn carousel + IG carousel → post across platforms → each platform's audience drives followers on all platforms → more followers = more thread ideas from audience questions → more threads
**Parts:** AI Agents (format conversion), APIs (multi-platform posting), Applications (design automation)
**Hat:** `[WHITE]`
**Build:** Twitter webhook on thread publish → AI conversion → Canva API carousel generation → multi-platform post → engagement tracking

### Robot 15: The Community Seed-and-Feed
**Loop:** Create community (Discord/Slack/Circle) → share daily valuable content → members invite others (incentivized with roles/access) → new members bring questions → questions become content ideas → more valuable content → more invites
**Parts:** Product (community platform), Users (members), AI Agents (content from questions), Applications (community tools)
**Hat:** `[WHITE]`
**Build:** Community platform API → question monitoring → AI content generation from questions → auto-post answers → invite tracking → role automation

### Robot 16: The Programmatic SEO Machine
**Loop:** Identify template-able search queries (e.g., "[tool] vs [tool]", "[thing] in [city]") → AI generates hundreds of pages from templates + data → Google indexes → long-tail traffic → traffic reveals new template patterns → more pages
**Parts:** APIs (keyword data, data sources), AI Agents (content generation), Applications (CMS), Product (website)
**Hat:** `[WHITE]` if genuinely useful content. `[GREY]` if thin/templated
**Build:** Keyword API → template engine → AI content fill → CMS API bulk publish → GSC monitoring → pattern identification

### Robot 17: The Live Stream Clip Factory
**Loop:** Go live weekly → AI records + transcribes in real-time → identifies clip-worthy moments → auto-generates clips during the stream → clips posted same day → clips drive viewers to next live → bigger live audience → better clips
**Parts:** AI Agents (transcription + clip identification), APIs (streaming + posting), Product (live content), Users (viewers)
**Hat:** `[WHITE]`
**Build:** OBS + streaming API → Whisper real-time → clip detection algorithm → auto-edit → immediate posting → next-live promotion

### Robot 18: The Testimonial Snowball
**Loop:** Customer achieves result → automation triggers review/testimonial request → AI formats testimonial into social content → posted as social proof → new prospects see proof → convert → achieve results → request THEIR testimonial
**Parts:** APIs (CRM triggers), AI Agents (formatting), Users (customers), Product (social proof content)
**Hat:** `[WHITE]`
**Build:** CRM milestone trigger → automated review request → AI testimonial formatting → social posting → conversion tracking

---

## EMAIL LIST GROWTH ROBOTS

### Robot 19: The Lead Magnet Machine
**Loop:** Identify top blog post by traffic → AI generates a lead magnet (checklist/template/cheat sheet) for that topic → embed opt-in on the post → visitors download → email captured → nurture sequence → subscribers share content → more traffic → identify next top post
**Parts:** APIs (analytics, email platform), AI Agents (lead magnet generation), Product (blog + email), Users (subscribers)
**Hat:** `[WHITE]`
**Build:** GA API → top content identification → AI lead magnet generator → opt-in embed → email automation → share tracking

### Robot 20: The Content Upgrade Factory
**Loop:** For every new blog post, AI auto-generates a content upgrade (PDF version, bonus tips, template) → inline opt-in captures email → new subscriber enters nurture → nurture drives them to more blog posts → they opt in for MORE upgrades → list compounds
**Parts:** AI Agents (upgrade generation), APIs (email + CMS), Product (blog), Users (readers)
**Hat:** `[WHITE]`
**Build:** CMS webhook on publish → AI content upgrade generator → opt-in form injection → email platform API → nurture sequence

### Robot 21: The Quiz Funnel
**Loop:** AI-powered quiz ("What type of [X] are you?") → user completes quiz → email captured for results → results page recommends products/content → user shares quiz result on social → friends take quiz → emails captured → loop
**Parts:** Product (quiz), APIs (email capture), Users (quiz takers who share), AI Agents (result personalization)
**Hat:** `[WHITE]`
**Build:** Quiz builder + email integration → social share buttons on results → UTM tracking → viral coefficient measurement

### Robot 22: The Webinar Replay Engine
**Loop:** Host live webinar → record → AI chops into highlight clips → clips posted as ads/organic content → viewers sign up for next webinar → attend → some don't attend but email captured → replay sent → nurture sequence → they attend NEXT webinar
**Parts:** Product (webinar), AI Agents (clip generation), APIs (email + ad platforms), Users (attendees)
**Hat:** `[WHITE]`
**Build:** Webinar platform API → AI highlight extraction → ad creative generation → email automation → registration tracking → attendance optimization

### Robot 23: The Free Tool Trap
**Loop:** Build simple free tool (calculator, generator, analyzer) → tool solves a small problem → requires email to save/export results → email captured → nurture promotes paid product → satisfied users share the free tool → more emails
**Parts:** Product (free tool), APIs (email capture), Users (tool users who share), AI Agents (tool maintenance)
**Hat:** `[WHITE]`
**Build:** Simple web app → email gate on export/save → nurture sequence → social share prompt → usage analytics

### Robot 24: The Exit Intent Rescue
**Loop:** Visitor about to leave site → exit intent popup with compelling offer → email captured → nurture sequence brings them back → they consume more content → share with others → new visitors → some try to leave → exit intent captures them
**Parts:** Product (website + popup), APIs (email platform), Applications (popup tool), Users (visitors)
**Hat:** `[WHITE]`
**Build:** Exit intent JS → dynamic offer based on page viewed → email capture → behavior-based nurture

### Robot 25: The Referral Tier System
**Loop:** New subscriber gets unique referral link → refer 3 friends = bonus content → refer 5 = exclusive access → refer 10 = free product → each referred friend gets THEIR OWN referral link → exponential growth
**Parts:** Product (referral program), APIs (email platform tracking), Users (subscribers), Applications (reward delivery)
**Hat:** `[WHITE]`
**Build:** Beehiiv/SparkLoop referral program → tiered reward automation → unique link generation → milestone triggers

### Robot 26: The Gated Community Play
**Loop:** Create exclusive community (free but email-gated) → members get daily value → invite-only creates FOMO → members get +1 invites → invitees must provide email → community grows → more value from more members → more invites
**Parts:** Product (community), APIs (email + community platform), Users (members), Applications (invite system)
**Hat:** `[WHITE]`
**Build:** Community platform → email-gated signup → invite code system → daily content automation → member growth tracking

### Robot 27: The Abandoned Cart Email Harvester
**Loop:** Visitor adds to cart but doesn't buy → email captured during checkout process → abandoned cart sequence fires → some convert → purchasers enter post-purchase sequence → they refer friends → friends visit → some abandon cart → emails captured
**Parts:** APIs (ecommerce platform + email), Product (store), Users (shoppers), AI Agents (email personalization)
**Hat:** `[WHITE]`
**Build:** Shopify/WooCommerce webhook → email automation → cart recovery sequence → post-purchase referral prompt

### Robot 28: The Waitlist FOMO Engine
**Loop:** Announce upcoming product/feature → waitlist captures email → show waitlist position publicly → FOMO drives more signups → each person on waitlist can "skip the line" by referring friends → friends join waitlist → viral growth
**Parts:** Product (waitlist page), APIs (email + referral tracking), Users (signups), Applications (position tracker)
**Hat:** `[WHITE]`
**Build:** Landing page → email capture → position display → referral skip-the-line mechanic → viral coefficient tracking

### Robot 29: The Newsletter Swap Network
**Loop:** Find newsletters with similar audience size → propose swap (you promote them, they promote you) → each newsletter gains subscribers from the other → both lists grow → qualify for swaps with BIGGER newsletters → even more subscribers
**Parts:** APIs (newsletter platforms), AI Agents (swap pitch writing), Users (subscribers), Applications (tracking)
**Hat:** `[WHITE]`
**Build:** Newsletter discovery → AI pitch generation → swap tracking → subscriber attribution → growth measurement

### Robot 30: The Social Proof Popup
**Loop:** Visitor on site → popup shows "John from NYC just signed up 2 minutes ago" → social proof triggers signup → new signup triggers the NEXT popup for the NEXT visitor → self-feeding social proof
**Parts:** Product (website), APIs (signup webhooks), Applications (popup tool like Proof/Fomo), Users (visitors)
**Hat:** `[WHITE]` if real data. `[GREY]` if fabricated
**Build:** Signup webhook → social proof popup service → real-time display → conversion tracking

### Robot 31: The PDF-to-Email Gateway
**Loop:** Create valuable PDF resources → rank them on Google for download-intent keywords → searcher finds PDF → email required to download → email captured → nurture sequence → subscriber creates content about PDF → more backlinks → higher Google ranking → more downloads
**Parts:** APIs (email + SEO tracking), AI Agents (PDF creation), Product (PDFs), Users (downloaders)
**Hat:** `[WHITE]`
**Build:** AI PDF generation → SEO-optimized landing pages → email gate → nurture → backlink monitoring

### Robot 32: The Micro-Commitment Ladder
**Loop:** Free micro-resource (1-page checklist, no email required) → reader gets value → prompted for email to get the FULL version → email captured → full version delivered → prompted to share for BONUS version → friend gets micro-resource → loop restarts
**Parts:** Product (tiered content), APIs (email), Users (readers who share), AI Agents (content tier generation)
**Hat:** `[WHITE]`
**Build:** Landing page funnel → progressive commitment steps → email capture at mid-point → share incentive → tracking

### Robot 33: The LinkedIn Article-to-Newsletter Bridge
**Loop:** Publish LinkedIn article → article gets distribution from LinkedIn algorithm → CTA drives to newsletter signup → newsletter delivers exclusive content → newsletter promotes next LinkedIn article → article gets more engagement → more newsletter signups
**Parts:** APIs (LinkedIn + email platform), Product (articles + newsletter), Users (LinkedIn audience)
**Hat:** `[WHITE]`
**Build:** LinkedIn publishing API → newsletter CTA insertion → email capture → newsletter automation → LinkedIn article promotion cycle

### Robot 34: The Webflow + Email Integration
**Loop:** Dynamic website content updates weekly → email notifies subscribers of new content → subscribers visit → some share → shared links bring new visitors → new visitors see email capture → subscribe → loop
**Parts:** APIs (CMS + email), Product (website), Users (subscribers), AI Agents (content updates)
**Hat:** `[WHITE]`
**Build:** CMS webhook on content update → email trigger → subscriber notification → visit tracking → capture optimization

---

## LEAD GENERATION ROBOTS

### Robot 35: The Power Dynamic Flip Ad
**Loop:** Run ad that frames lead gen as a protective service ("Is someone already listing your property?") → prospect fills form out of fear/curiosity → sales call positions you as helper → close → happy client refers others → referrals see ad → loop
**Parts:** APIs (ad platform + CRM), AI Agents (ad copy), Users (prospects), Product (the "check")
**Hat:** `[GREY]` — framing is manipulative but legal
**Build:** Meta/Google Ads API → landing page → CRM webhook → sales sequence → referral request automation

### Robot 36: The Competitor Review Interceptor
**Loop:** Monitor when competitor gets negative reviews → auto-trigger ad targeting that competitor's audience → ad positions you as the alternative → lead captured → converted → happy customer leaves YOU a positive review → more social proof → more conversions
**Parts:** APIs (review monitoring + ad platform), AI Agents (ad generation), Users (competitor's unhappy customers)
**Hat:** `[GREY]` — targeting competitor's audience is aggressive but legal
**Build:** Review monitoring API → negative review trigger → dynamic ad creation → landing page → CRM → review request automation

### Robot 37: The LinkedIn Engagement-to-Lead Pipeline
**Loop:** Post valuable content on LinkedIn → engage commenters with thoughtful replies → AI identifies high-value commenters (title, company, fit) → auto-send connection request with personalized note → connection accepts → nurture via DMs → book call → close
**Parts:** APIs (LinkedIn), AI Agents (commenter analysis + personalization), Users (commenters), Applications (CRM)
**Hat:** `[GREY]` — automated LinkedIn outreach bends TOS
**Build:** LinkedIn API → engagement monitoring → AI lead scoring → personalized connection request → DM sequence → calendar booking

### Robot 38: The Chatbot Qualifier
**Loop:** Website visitor arrives → AI chatbot engages → qualifies through conversation → captures email + needs → books call if qualified → call converts → client refers friend → friend visits site → chatbot engages
**Parts:** Product (chatbot), AI Agents (conversation + qualification), APIs (calendar + CRM), Users (visitors)
**Hat:** `[WHITE]`
**Build:** AI chatbot (Claude API) → qualification logic → CRM integration → calendar booking API → referral tracking

### Robot 39: The Scrape-and-Reach Engine
**Loop:** Scrape industry directories/LinkedIn for ideal customer profiles → AI writes personalized outreach → send via email/LinkedIn → responses enter CRM → nurture non-responders → converted clients provide referrals + testimonials → testimonials improve outreach conversion → more outreach
**Parts:** APIs (scraping + email + CRM), AI Agents (personalization), Users (prospects), Applications (outreach tools)
**Hat:** `[GREY]` — scraping + cold outreach can violate TOS/GDPR
**Build:** Scraping tool → AI personalization → Instantly/Apollo outreach → CRM → testimonial collection → outreach optimization

### Robot 40: The Case Study Generator
**Loop:** Client achieves result → AI auto-generates case study (before/after, metrics, quotes) → case study published on site → ranks for "[industry] case study" searches → prospect finds case study → books call → becomes client → achieves result → generates NEXT case study
**Parts:** AI Agents (case study writing), APIs (CMS + SEO), Users (clients), Product (case studies)
**Hat:** `[WHITE]`
**Build:** CRM milestone trigger → AI case study generator → client approval workflow → CMS publish → SEO optimization → lead tracking

### Robot 41: The Retargeting Loop
**Loop:** Visitor hits site but doesn't convert → pixel fires → retargeting ad follows them across platforms → ad brings them back → they consume more content → still don't convert → new retargeting ad with different angle → eventually convert → their visit data improves targeting for next prospects
**Parts:** APIs (ad platforms + pixel), AI Agents (ad creative rotation), Users (visitors), Applications (ad platforms)
**Hat:** `[WHITE]`
**Build:** Facebook Pixel + Google tag → audience segmentation → AI ad creative generation → sequential retargeting → conversion tracking → audience refinement

### Robot 42: The Job Board Trojan
**Loop:** Post attractive job listings on job boards (even if not hiring) → candidates apply with contact info → auto-respond with "role filled but check our services" → some convert to customers → customers hire through you later → post more listings
**Parts:** APIs (job board), AI Agents (listing creation), Users (applicants), Product (services)
**Hat:** `[BLACK]` — deceptive if not actually hiring
**Build:** Job board API → automated listing → auto-response sequence → CRM → service conversion tracking

### Robot 43: The Calculator Lead Magnet
**Loop:** Build industry-specific calculator (ROI calculator, savings estimator, sizing tool) → promote via SEO + ads → user inputs their data to get result → email required for detailed report → email captured → AI-personalized follow-up based on their inputs → close → refer → more calculator users
**Parts:** Product (calculator), APIs (email + CRM), AI Agents (personalized follow-up), Users (calculator users)
**Hat:** `[WHITE]`
**Build:** Web calculator → data capture → AI analysis of inputs → personalized email sequence → CRM → sales tracking

### Robot 44: The Event Attendance Machine
**Loop:** Host free virtual event (workshop, AMA, demo) → registration captures email → attendees get value → post-event sequence nurtures → some convert → clients invited to NEXT event as speakers/testimonials → their audience registers → more attendees
**Parts:** Product (events), APIs (event platform + email), Users (attendees + speaker-clients), AI Agents (event content)
**Hat:** `[WHITE]`
**Build:** Event platform → registration + email capture → attendance tracking → post-event nurture → client-as-speaker pipeline

### Robot 45: The Review Response Revenue Loop
**Loop:** Customer leaves Google review → AI generates thoughtful response → response visible to all Google searchers → searchers see engaged business → click through to site → some become leads → leads convert → happy clients leave reviews → loop
**Parts:** APIs (Google Business), AI Agents (response generation), Users (reviewers + searchers), Product (business listing)
**Hat:** `[WHITE]`
**Build:** Google Business API → review notification → AI response generator → response posting → click tracking → lead attribution

### Robot 46: The Cold-to-Warm Bridge
**Loop:** Cold prospect list → AI sends value-first email (free resource, insight, data) → prospect opens → tagged as "warm" → warm sequence offers consultation → some book → consultation converts → client refers warm contacts → new warm leads enter sequence
**Parts:** APIs (email + CRM), AI Agents (email personalization), Users (prospects), Product (value resources)
**Hat:** `[WHITE]` if opted-in list. `[GREY]` if cold email
**Build:** Email platform → segmentation → AI value-first content → engagement scoring → warm transition → consultation booking → referral system

### Robot 47: The Directory Domination Play
**Loop:** List business on every relevant directory (50+) → each listing = backlink + potential lead source → directories rank in Google → searchers find listings → click through to site → some convert → positive reviews on directories boost listing → more clicks → more leads
**Parts:** APIs (directory platforms), AI Agents (listing optimization), Users (directory searchers), Product (business listings)
**Hat:** `[WHITE]`
**Build:** Directory submission automation → listing optimization → review collection → click tracking → ROI measurement per directory

### Robot 48: The Partner Referral Engine
**Loop:** Identify complementary businesses → propose referral partnership (you refer to them, they refer to you) → CRM tracks referrals both ways → each successful referral strengthens the partnership → partners introduce you to THEIR partners → referral network expands
**Parts:** APIs (CRM), Users (partners + their clients), Applications (referral tracking), AI Agents (partner identification)
**Hat:** `[WHITE]`
**Build:** CRM partner tracking → automated referral attribution → commission/reciprocity tracking → partner network expansion → monthly reporting

### Robot 49: The Intent Signal Sniper
**Loop:** Monitor intent signals (Google searches, LinkedIn activity, job changes, funding announcements) → AI identifies prospects showing buying intent → auto-trigger personalized outreach → prospect is ready to buy → faster close → CRM data improves intent signal accuracy → better targeting
**Parts:** APIs (intent data providers, LinkedIn, Crunchbase), AI Agents (personalization), Applications (CRM + outreach)
**Hat:** `[GREY]` — data sourcing may push boundaries
**Build:** Bombora/G2/LinkedIn intent API → AI scoring → personalized outreach → CRM → conversion data feedback → model improvement

### Robot 50: The Trojan Tool
**Loop:** Build genuinely useful free tool for your target market → tool requires account creation → tool embeds YOUR branding + backlinks → users share tool with colleagues → colleagues create accounts → tool usage data reveals buying intent → sales outreach to high-usage accounts → convert → users keep using tool → keep sharing
**Parts:** Product (free tool), APIs (user tracking + CRM), Users (tool users who share), AI Agents (intent identification)
**Hat:** `[WHITE]` — the CGA skill itself is a Trojan Tool for CMNDSHFT
**Build:** Web app → account system → usage analytics → intent scoring → sales trigger → backlink tracking

---

## How to Use This List

1. **During onboarding:** After identifying the bottleneck (traffic / conversion / retention), the CGA recommends 3-5 relevant robots from this list
2. **In operational mode:** The CGA adapts these templates to the specific business, mapping available tools and integrations to the robot parts
3. **The CGA generates a build prompt** for each approved robot — a deployment-ready spec that can be handed to Claude Code for execution

**The robot test always applies:**
- Can you turn it off?
- Is it running without humans?
- Does each cycle's output feed the next input?
