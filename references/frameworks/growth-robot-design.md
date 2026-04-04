# Growth Robot Design — The ROBOT Framework

> Source: "Growth Robot" by Bronson Taylor
> Layer: Immutable Knowledge Base

---

## What is a Robot?

**ROBOT** = **R**epeatable, **O**rdered, **B**usiness **O**perations, utilizing **T**echnology

A robot is a systematic, technology-powered loop that drives business growth without requiring the architect to be a cog in the machine.

---

## The Four Properties

### 1. Repeatable

The genius is in repeatability. If it's a one-off event, it's not a robot. Robots are loops that perpetuate without end. The output of one cycle becomes the input for the next.

### 2. Ordered

Steps build on each other in sequence. Can't do step 4 before step 1. The order matters — each step depends on the output of the previous step.

### 3. Business Operations

Every step is chosen for its impact on the business. Not automation for automation's sake — automation for business growth. If a robot stops generating positive ROI, dismantle it.

### 4. Technology

Traditional processes use employees as primary input. Robots use instantaneous technologies. When humans are needed, use virtual assistants (or AI agents) managed via technology.

---

## The 7 Types of Robot Parts

### 1. APIs

Data flow between applications. Thousands available (Twilio, social APIs, email APIs, etc.). Advanced usage includes undocumented APIs and screen scraping to create your own API endpoints.

### 2. Applications

Sometimes you need the full app, not just the API. Dashboards, CRMs, admin panels serve as robot components where human review or action is needed within the loop.

### 3. Users

Customer actions that feed the robot — email input, form fills, purchases, clicks. This is a balancing act: don't ask for too much data or you'll break the loop with friction.

### 4. Product

Event triggers within your own product. Milestone tracking, usage-based triggers, feature-based flows. Appears in most robots because the product itself generates the signals that drive the loop.

### 5. Virtual Assistants / AI Agents

Flexible intelligence for steps APIs can't handle. Research, judgment calls, nuanced tasks. Use VA companies for continuity (or in the CGA context, AI agents replace most VA roles). These handle the "gray area" steps that require reasoning.

### 6. Partnerships

Other companies as loop participants. Example: competitor cross-referral on cancellation — when a customer cancels, route them to a partner product and receive referral credit. Rare but potentially the most powerful part type.

### 7. Employees

Last resort. Only for high-ROI robots where human expertise is truly required (e.g., complex sales calls, strategic negotiations). Never let the architect or mechanic become a cog in the robot.

---

## The Two Roles

### Architect

The mastermind who designs robots. Uses creativity + technology knowledge to visualize new robots. Creates blueprints. The architect should **NEVER** become a cog in their own robot. Don't be a cog. Be a creator.

### Mechanic

Translates blueprints into working robots. Usually needs development skills (or in the CGA context, automation and integration skills). Must also never become a cog. Complexity doesn't equal more growth — simple robots can be the most powerful.

---

## Robot Design Process

1. **Define the desired END outcome** — What business result does this robot produce?
2. **Work BACKWARDS from there** — What has to happen right before the end? And before that?
3. **Identify which of the 7 parts are needed at each step** — API? User action? AI agent?
4. **Map the ordered sequence** — Lay out every step in exact order
5. **Find the loop** — Where does the output become new input? This is what makes it a robot, not a process
6. **Test run manually before automating** — Walk through each step by hand to validate the logic
7. **Deploy and measure** — Launch, track ROI, and iterate

---

## Example Robot: Growth Hacker TV

Full working example from the book demonstrating all four properties:

1. **User** visits site → plays video
2. After time increment, email popup appears → **User** enters email
3. Email → **Rapportive API** → returns Twitter handle
4. Twitter handle → **Twitter API** → returns list of followers
5. Followers → **Klout API** → ranked by influence score
6. Most influential followers listed on **admin panel** (Application)
7a. Followers' tweets are favorited from @growthhackertv (**API**)
7b. Followers get @replied from @growthhackertv (**API**)
7c. **Virtual assistants** find follower emails and send outreach
8. Followers click links → arrive on site → **process begins again** (THE LOOP)

This is a ROBOT: repeatable (loops endlessly), ordered (each step feeds the next), focused on business growth (audience building), powered by technology (APIs + automation).

---

## Key Principles

> "Sometimes it is helpful to think of what action you want to occur at the END of your robot when it has run, and then work backwards from there to discover what pieces are necessary."
> — Bronson Taylor

- **Don't be a cog.** The architect designs robots. The moment you become a step in your own robot, you've failed.
- **Simple beats complex.** A 3-step robot that runs 1,000 times beats a 20-step robot that breaks constantly.
- **ROI is the only measure.** If a robot doesn't generate positive business outcomes, kill it.
- **Find the loop.** Every robot must have a loop — output feeds back as input. No loop = just a process, not a robot.
- **Technology multiplies.** Traditional marketing adds. Technology-powered marketing multiplies.

---

## CGA Application Notes

When designing growth robots for clients:

- **AI agents replace VAs** in most steps — faster, cheaper, always available
- **Modern APIs** are far more capable than when this framework was written — LLM APIs, webhook platforms, and no-code tools expand what's possible
- **The framework is timeless** — the 7 part types and 4 properties still hold. Only the specific technologies change.
- **Always start with the business outcome**, never with the technology. "What growth do we need?" comes before "What can we automate?"
