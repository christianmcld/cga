# Case Study: Zynga — The Decoy-as-Distribution Robot

**Hat:** `[GREY]`
**Type:** ROBOT (literal technical automation, self-feeding loop)
**Principle:** Re-engineer the pricing decoy so the "middle option" becomes your viral distribution engine

## What Happened

FarmVille, MafiaWars, and Zynga Poker dominated Facebook gaming. At peak, FarmVille had 83M monthly active users. Zynga's growth was powered by a specific product mechanic that weaponized the classic pricing decoy.

## The Robot

```
1. User plays free game → hits a wall (needs resources/lives/progress)
2. Product presents 3 choices:
   - GRIND (slow — costs time)
   - SPAM (free — costs social capital, invite friends)
   - PAY (instant — costs money)
3. Most users choose SPAM → click invite → Facebook API sends notifications
4. Friends receive invitations → curiosity/obligation pulls them in
5. New users play → hit the same wall → GRIND / SPAM / PAY
6. Loop repeats exponentially
```

## Why It's a Real Robot

- **Autonomous:** Built into the product code, runs without human intervention
- **Self-feeding:** Each user's spam invitations feed new users into the same loop
- **Self-growing:** Each cycle brings more users than it consumes (viral K >> 1.0)
- **Technical:** Facebook API integration, product event triggers, automated notifications

## The Growth Hack

The classic pricing decoy: Small $3, Medium $6.50, Large $7. The medium exists to make the large look like a deal.

Zynga's twist: The "middle option" (SPAM) wasn't designed to generate revenue — it was designed to generate **growth**. Revenue came from the small percentage who chose PAY. Growth came from the majority who chose SPAM.

They turned a pricing psychology trick into a viral distribution engine.

## Results

- **Peak users:** 83M monthly active users (FarmVille alone)
- **Viral coefficient:** Massively above 1.0 (each user spammed 10-20+ friends)
- **Revenue model:** Small % of payers subsidized by massive user base
- **IPO valuation:** $7B (2011)

## The Collapse

Facebook rewrote its notification policies specifically because of Zynga. When the platform shut down the spam loop, Zynga's growth engine died. Stock cratered from $14.69 to $2.09.

## Risk Matrix

| Dimension | Rating | Note |
|-----------|--------|------|
| Legality | **WHITE** | Fully legal — users chose to invite |
| Platform TOS | **GREY → BLACK** | Facebook eventually killed it with policy changes |
| Reputation | **GREY** | "Annoying" brand perception, user resentment |
| Reversibility | **GREY** | Once Facebook shut the door, growth engine died instantly |
| Detection | **WHITE** | Fully visible by design |

## Key Principles for the CGA

### 1. The Decoy-as-Distribution Hack
Take any pricing/choice architecture and ask: "Can one of these options be designed to spread the product instead of generate revenue?" Revenue and growth don't have to come from the same option.

### 2. Platform Dependency Risk
**Never build your only growth robot on rented land.** Zynga's entire engine was a feature of Facebook's notification system. When Facebook patched it, Zynga lost everything. Always diversify your growth robots across platforms you control.

### 3. The Psychology Stack
Zynga stacked multiple psychology triggers:
- **Progress** (trigger #2) — progress bars, level-ups, achievements
- **Fear** (trigger #5) — FOMO, friends advancing without you
- **Social Proof** (trigger #6) — "Your friend just harvested their farm"
- **Contrast** (trigger #4) — free/slow vs free/spam vs paid/instant

The combination was more powerful than any single trigger.
