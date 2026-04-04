# Risk Matrix — Hat Classification System

Every tactic, play, and growth robot is tagged with a hat color. This file defines the classification criteria.

## Hat Colors

### [WHITE] — Safe & Sustainable
Legal, ethical, platform-compliant. Execute freely.

### [GREY] — Effective but Risky
Legal but borderline. May bend platform TOS. Requires explicit CEO approval before execution.

### [BLACK] — Aggressive & Dangerous
May violate laws or platform TOS. Presented as knowledge only. Requires explicit acknowledgment of risks before any action.

## Classification Dimensions

| Dimension | WHITE | GREY | BLACK |
|-----------|-------|------|-------|
| **Legality** | Fully legal in all jurisdictions | Legal but gray area (e.g., CAN-SPAM edge cases) | May violate laws (GDPR, CAN-SPAM, CFAA, etc.) |
| **Platform TOS** | Fully compliant | Bends rules, not explicitly banned yet | Explicitly violates TOS |
| **Reputational Risk** | None — would be proud if published | Moderate — could look bad if discovered | Severe — brand damage if exposed |
| **Reversibility** | Fully reversible, no lasting damage | Partially reversible, some cleanup needed | Difficult or impossible to undo |
| **Detection Likelihood** | N/A — nothing to detect | Low to Medium | Medium to High |

## Scoring Process

When evaluating a tactic:

1. Score each dimension independently (WHITE / GREY / BLACK)
2. The overall hat color = the WORST score across all dimensions
3. If ANY dimension is BLACK, the play is BLACK
4. If ANY dimension is GREY (and none are BLACK), the play is GREY
5. Only if ALL dimensions are WHITE is the play WHITE

## Approval Requirements

- **WHITE:** Recommend freely. No gate required.
- **GREY:** Present with full risk matrix expanded. Require CEO to explicitly say "approved" before generating build prompt.
- **BLACK:** Present as educational knowledge. Full risk matrix. Require CEO to acknowledge: "I understand the risks and want to proceed." Double-confirm before generating build prompt.

## Dashboard Display

- Tags show as colored badges: [WHITE] [GREY] [BLACK]
- Clicking a tag expands the full risk matrix for that specific play
- Each dimension shows its individual score with a one-line explanation
