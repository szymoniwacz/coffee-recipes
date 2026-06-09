# V60 — Balanced

## Quick Brew Card

- **Dose:** 15 g · **Water:** 200 g · **Grind:** Comandante 24 clicks · **Temp:** 92°C · **Brew time:** TBD
- **Pour schedule:** Bloom 30 g → +45 g (75 g) → +45 g (120 g) → +45 g (165 g); remaining to 200 g TBD

### Taste Check
- Rest after brewing: not documented
- Best first sip: not documented
- Best taste range: not documented

## Short Version

1. Bloom 30 g (time TBD).
2. Pour 45 g three times (75 → 120 → 165 g cumulative).
3. Top up to 200 g total (final pour not documented).

## Status

- Status: tested
- Last updated: 2026-06-03

## Coffee

- Name: Xin Chao Hanoi (100% Robusta, speciality)
- Bean: Robusta
- Origin: Vietnam
- Process: Honey
- Roast level: Medium
- Roaster: 1996 Coffee

## Goal

More interesting, more complex cup at the cost of some body.

Reference profile: *24 kliki* — even three pours after bloom at Comandante 24 clicks.

## Equipment

- Brewer: V60
- Filter: not documented
- Grinder: Comandante
- Kettle: not documented
- Scale: not documented

## Parameters

- Coffee dose: 15 g
- Water amount: 200 g
- Brew ratio: 1:13.3 (15 g : 200 g)
- Water temperature: 92°C
- Grind size: Comandante 24 clicks
- Water type: not documented

## Pour Structure

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom | 30 g | 30 g | 0:00 | not documented | bloom time not in source |
| Pour #1 | 45 g | 75 g | not documented | not documented | |
| Pour #2 | 45 g | 120 g | not documented | not documented | |
| Pour #3 | 45 g | 165 g | not documented | not documented | listed pours sum to 165 g; target water 200 g |
| Pour #4 | — | — | — | — | not applicable |
| Pour #5 | — | — | — | — | not applicable |

## Pouring Technique

- Pour style: not documented
- Center pour / circular pour: not documented
- Agitation: not documented
- Swirl: not documented
- Stirring: not documented
- Flow rate: not documented
- Bed shape target: not documented

## Timing

- Bloom time: not documented
- Drawdown time: not documented
- Total brew time: not documented

## Result

- Sweetness: not documented
- Body: lower — lacked some body
- Acidity: not documented
- Bitterness: not documented
- Clarity: not documented
- Strength: not documented
- Aftertaste: not documented
- Taste after cooling: not documented
- Complexity: high — more interesting, more complex

## Serving And Tasting

- Recommended resting time after brewing: not documented
- First tasting point: not documented
- Optimal tasting temperature: not documented
- Flavor evolution as coffee cools: not documented

## Extraction Logic

- **24 clicks:** coarser than [Strong](./strong.md) (25–27) and [Stable](./stable.md) (25) — favors complexity over body.
- **92°C:** standard temperature in this V60 line.
- **Three equal +45 g pours after bloom:** even split; cumulative from source reaches 165 g before any undocumented top-up to 200 g.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness | [Stable](./stable.md); [Strong](./strong.md) at 91°C |
| More body | [Stable](./stable.md); finer than 24 clicks |
| More strength | [Strong](./strong.md) |
| Less bitterness | not documented |
| Less acidity | not documented |
| Less watery taste | not documented |
| Better taste after cooling | [Stable](./stable.md) |
| More complexity | keep 24 clicks; this recipe’s strength |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Watery / thin | underextraction — too coarse | finer; compare [Stable](./stable.md) |
| Harsh bitterness | overextraction | coarser; lower temperature |
| Sourness / acidity | underextraction | finer |
| Slow drawdown | too fine | coarser |
| Fast drawdown | too coarse | finer |
| Too little body | expected at 24 clicks | [Stable](./stable.md) or [Strong](./strong.md) |

## Historical Notes

- Original source: `## V60 #2 — 24 kliki`.
- Former filenames: `24-clicks.md`, `podstawowy-pour-over.md`.
- **Pour total note:** source lists three +45 g pours after 30 g bloom (165 g cumulative); water target is 200 g — remaining distribution not in source.
- Rename file after cup log if “balanced” does not match Result.

## Evidence

| Item | Value | Source | Confidence |
|---|---|---|---|
| Parameters, pour increments, Result | As documented | Robusta Honey source of truth (2026-06-03) | **High** |
| Cumulative totals 75 / 120 / 165 g | Arithmetic from bloom + pours | Derived from source | **High** |
| Gap 165 g → 200 g water | Not in source | — | — |
| Bloom time, total brew time, pouring technique | not documented | No source | — |

**Overall confidence:** **High** (parameters and pours); **Medium** for full 200 g pour schedule

## Related Recipes

- See also:
  - [V60 — Sweetness + body](./sweetness-body.md)
  - [V60 — Stable](./stable.md) — 25 clicks, 5 pours
  - [V60 — Strong](./strong.md)
  - [V60 Switch — Immersion](../v60-switch/immersion-sweetness-body.md)
  - [Aeropress Prism — Sweet & Clean](../aeropress-prism/sweet-clean.md)

## Future Experiments

- Log how the cup reaches 200 g (fourth pour or adjusted pours).
- Compare 24 clicks vs 25 ([Stable](./stable.md)) on same dose and water.
