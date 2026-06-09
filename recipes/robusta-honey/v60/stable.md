# V60 — Stable

## Quick Brew Card

- **Dose:** 15 g · **Water:** 200 g · **Grind:** Comandante 25 clicks · **Temp:** 92°C · **Brew time:** 2:45–3:10
- **Pour schedule:** Bloom 30 g (45 s) → +45 g (75 g) → +40 g (115 g) → +40 g (155 g) → +45 g (200 g)

### Taste Check
- Rest after brewing: not documented
- Best first sip: not documented
- Best taste range: not documented

## Short Version

1. Bloom 30 g for 45 s.
2. Pour 45 g, 40 g, 40 g, then 45 g (200 g total).
3. Target finish between 2:45 and 3:10.

## Status

- Status: baseline
- Last updated: 2026-06-03

## Coffee

- Name: Xin Chao Hanoi (100% Robusta, speciality)
- Bean: Robusta
- Origin: Vietnam
- Process: Honey
- Roast level: Medium
- Roaster: 1996 Coffee

## Goal

Very full body, lots of sweetness, and good taste after cooling.

**Current best V60 recipe** in the source list. Original title: *25 klików, 5 zalań* — five pour stages including bloom (four pours after bloom).

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
- Grind size: Comandante 25 clicks
- Water type: not documented

## Pour Structure

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom | 30 g | 30 g | 0:00 | 0:45 | 45 s bloom |
| Pour #1 | 45 g | 75 g | not documented | not documented | |
| Pour #2 | 40 g | 115 g | not documented | not documented | |
| Pour #3 | 40 g | 155 g | not documented | not documented | |
| Pour #4 | 45 g | 200 g | not documented | not documented | |
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

- Bloom time: 45 s
- Drawdown time: not documented
- Total brew time: 2:45–3:10

## Result

- Sweetness: high — lots of sweetness
- Body: very high — very full body
- Acidity: not documented
- Bitterness: not documented
- Clarity: not documented
- Strength: not documented
- Aftertaste: not documented
- Taste after cooling: good — good after cooling

## Serving And Tasting

- Recommended resting time after brewing: not documented
- First tasting point: not documented
- Optimal tasting temperature: not documented
- Flavor evolution as coffee cools: not documented

## Extraction Logic

- **25 clicks:** finer than [Balanced](./balanced.md) (24) — supports body and sweetness.
- **92°C:** matches other high-performing V60 variants.
- **Four pours after bloom (45 + 40 + 40 + 45 g):** phased schedule to 200 g; more pours than [Strong](./strong.md) (3 pours).

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness | already high — avoid coarser than 25 |
| More body | already very full — compare [Strong](./strong.md) for strength |
| More strength | [Strong](./strong.md) — 91°C, 25–27 clicks |
| Less bitterness | coarser than 25 — not tested |
| Less acidity | not documented |
| Less watery taste | not documented |
| Better taste after cooling | already good — primary reference |
| More complexity | [Balanced](./balanced.md) at 24 clicks |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Watery / thin | underextraction — too coarse, incomplete pours | verify 25 clicks; full pour table to 200 g |
| Harsh bitterness | overextraction — too fine | coarser than 25 — not tested |
| Sourness / acidity | underextraction | finer; full 45 s bloom |
| Slow drawdown | too fine at 25 | coarser — watch body loss |
| Fast drawdown | too coarse | finer toward 25 |

## Historical Notes

- Original source: `## V60 #3 — 25 klików, 5 zalań` — noted as one of the current best V60 recipes.
- Former filenames: `25-clicks-5-pours.md`, `piec-zalan.md`.
- [Syphon — Stable + bite](../syphon/stable-bite.md) shares “stable” naming but is a **different method**.
- Spec examples (25 vs 26 clicks body trade-offs) were **not** added — not in source.

## Evidence

| Item | Value | Source | Confidence |
|---|---|---|---|
| Parameters, pour table, timing, Result, “best” note | As documented | Robusta Honey source of truth (2026-06-03) | **High** |
| Pour start/end times, pouring technique | not documented | No source | — |

**Overall confidence:** **High**

## Related Recipes

- See also:
  - [V60 — Balanced](./balanced.md)
  - [V60 — Strong](./strong.md)
  - [V60 — Sweetness + body](./sweetness-body.md)
  - [Syphon — Stable + bite](../syphon/stable-bite.md) — different method
  - [V60 Switch — Immersion](../v60-switch/immersion-sweetness-body.md)

## Future Experiments

- Log pour start/end times per stage.
- Document drawdown split; compare with [Balanced](./balanced.md) on complexity.
