# V60 — Strong

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

Strong cup with much body, not watery, and good sweetness.

Original source title: *Mocna, 3 zalania* — three pours after bloom for a dense, full cup.

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
- Water temperature: 91°C
- Grind size: Comandante 25–27 clicks (usually 25)
- Water type: not documented

## Pour Structure

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom | 30 g | 30 g | 0:00 | 0:45 | 45 s bloom |
| Pour #1 | 60 g | 90 g | not documented | not documented | |
| Pour #2 | 55 g | 145 g | not documented | not documented | |
| Pour #3 | 55 g | 200 g | not documented | not documented | |
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

- Bloom time: 45 s
- Drawdown time: not documented
- Total brew time: 2:45–3:10

## Result

- Sweetness: good — good sweetness
- Body: high — much body
- Acidity: not documented
- Bitterness: not documented
- Clarity: not documented
- Strength: high — strong, not watery
- Aftertaste: not documented
- Taste after cooling: not documented

## Extraction Logic

- **91°C:** slightly cooler than 92°C V60 variants — supports sweetness without a watery cup.
- **25–27 clicks (usually 25):** finer range for strength and body vs 24-click recipes.
- **3 pours after bloom (60 + 55 + 55 g):** phased pours to 200 g; larger first pour after bloom.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness | compare [Stable](./stable.md); slightly coarser in 25–27 range |
| More body | [Stable](./stable.md) — 5-pour profile |
| More strength | stay at 25 clicks; full 200 g |
| Less bitterness | coarser (26–27); slightly lower temperature — not tested |
| Less acidity | not documented |
| Less watery taste | already strong / full — avoid coarser grind |
| Better taste after cooling | compare [Stable](./stable.md) |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Watery / thin | underextraction — too coarse, too fast pours | finer (25); extend bloom |
| Harsh bitterness | overextraction — too fine, too hot | coarser; 91°C or lower |
| Sourness / acidity | underextraction | finer; full pours to 200 g |
| Slow drawdown | too fine | coarser in 25–27 range |
| Fast drawdown | too coarse | finer toward 25 |

## Historical Notes

- Original source: `## V60 #1 — Mocna, 3 zalania`.
- Former filenames: `mocna-3-zalania.md`, `mocna-trzy-zalania.md`, `strong-3-pours.md`.
- **Recommended use:** strong cup / morning.
- Consolidated duplicate files into this profile-based name.

## Evidence

| Item | Value | Source | Confidence |
|---|---|---|---|
| Parameters, pour table, timing, Result | As documented | Robusta Honey source of truth (2026-06-03) | **High** |
| Pour start/end times, pouring technique | not documented | No source | — |
| Xin Chao Hanoi; Robusta, Vietnam, Honey, Medium; 1996 Coffee | Repository coffee spec | All recipes in `robusta-honey/` | **High** |

**Overall confidence:** **High**

## Related Recipes

- See also:
  - [V60 — Balanced](./balanced.md)
  - [V60 — Stable](./stable.md)
  - [V60 — Sweetness + body](./sweetness-body.md)
  - [V60 Switch — Immersion, sweetness + body](../v60-switch/immersion-sweetness-body.md)

## Future Experiments

- Log pour start/end times per stage.
- Record drawdown split and taste after cooling.
