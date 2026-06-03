# Template compliance report

Migration date: 2026-06-03  
Source of truth: `coffee-recipe-template-spec.md` and `templates/*-template.md`

## Templates created

| File | Method |
|------|--------|
| `templates/v60-template.md` | V60 pour-over |
| `templates/v60-switch-template.md` | V60 Switch |
| `templates/aeropress-prism-template.md` | Aeropress + Prism |
| `templates/aeropress-paper-template.md` | Aeropress + paper |
| `templates/syphon-template.md` | Syphon 3-cup |
| `templates/electric-moka-pot-template.md` | Electric moka pot |

Removed: `templates/recipe-template.md` (generic) — replaced by method-specific templates.

## Recipes updated

| Recipe file | Template | Status before → after |
|-------------|----------|-------------------------|
| `v60/strong.md` | v60 | migrated |
| `v60/balanced.md` | v60 | migrated |
| `v60/stable.md` | v60 | migrated |
| `v60/sweetness-body.md` | v60 | migrated |
| `v60-switch/immersion-sweetness-body.md` | v60-switch | already compliant; verified |
| `aeropress-prism/sweet-clean.md` | aeropress-prism | migrated |
| `aeropress-prism/killer.md` | aeropress-prism | migrated |
| `aeropress-paper/paper-filter.md` | aeropress-paper | migrated |
| `syphon/sweet.md` | syphon | migrated |
| `syphon/stable-bite.md` | syphon | migrated |
| `electric-moka-pot/current-baseline.md` | electric-moka-pot | migrated |
| `electric-moka-pot/stronger-concentrated.md` | electric-moka-pot | migrated |

**Total:** 12 recipes, 6 templates. Filenames and titles unchanged.

## Unknown fields per recipe

### V60 — Strong (`strong.md`)

- Parameters: dose, water, ratio, temperature, grind, water type
- Pour Structure: all rows (intent: 3 pours — amounts/times unknown)
- Pouring Technique: all
- Timing: all
- Result: all sensory fields
- Most Warning Signs / Tuning rows

### V60 — Balanced (`balanced.md`)

- Dose, water, ratio, temperature, water type
- Full pour table and technique
- Timing, Result
- Grind known: 24 clicks

### V60 — Stable (`stable.md`)

- Same as balanced; grind 25 clicks; intent 5 pours
- Full pour amounts/times unknown

### V60 — Sweetness + body (`sweetness-body.md`)

- Dose, ratio (if dose ≠ 15 g), temperature, pour breakdown
- Water amount known: **190 g**; grind **24 clicks**
- Result: all (target profile documented, not tested on V60)

### V60 Switch — Immersion (`immersion-sweetness-body.md`)

- Coffee: origin, process, roast
- Filter, kettle, water type
- Agitation fields
- Bitterness, clarity, strength, aftertaste, taste after cooling
- Drawdown split after release; reference point for 1:45 timer

### Aeropress Prism — Sweet & Clean

- Setup: orientation, rinse, preheat
- Pressure level, stop at hiss
- Acidity, oiliness, taste after cooling

### Aeropress Prism — Killer

- Plunge start (exact), plunge duration, total time
- Setup fields; clarity; several Result subfields

### Aeropress — Paper filter

- Water temperature; number of filters; setup
- Plunge start (exact), total time; sweetness

### Syphon — Sweet

- Temperature; heat levels; drawdown duration
- Body, acidity, aroma; taste after cooling

### Syphon — Stable + Bite

- Temperature; heat levels; time reference for 20 s / 40–45 s
- Clarity; drawdown metrics; taste after cooling

### Moka — Current baseline

- Origin/process/roast; basket touches water; valve level
- Sweetness, body, acidity, clarity; cycle time; taste after cooling

### Moka — Stronger

- **Entire workflow**, shutdown cue, yield (all unknown)
- Water start, preparation steps (assumptions noted as not tested)
- Most Result except documented contrast vs baseline

## Preservation checklist

- [x] Historical Notes retained (including file rename notes, A/B vs other recipes)
- [x] Documented tasting results only (no invented cup notes)
- [x] Brew ratios where dose + water known
- [x] Workflow steps embedded in method sections or Historical Notes where template uses tables
- [x] Related Recipes / cross-links
- [x] Repeatability and use-case text → Historical Notes / Future Experiments

## Recommended tests (next brew session)

### V60 (all four)

1. Record **dose, temperature, and full Pour Structure table** (g per pour, cumulative g, start/end times).
2. Document **drawdown** and **taste after cooling** for comparison across strong / balanced / stable / sweetness-body.
3. For `sweetness-body.md`: brew with **15 g + 190 g** if that matches Switch A/B intent.

### V60 Switch

1. Fix timer reference: **1:45 from which event** (first pour vs valve close).
2. Note any **stir/swirl** before opening valve.

### Aeropress

1. Paper: measure **water temperature** and **exact plunge start** after 2 min steep.
2. Killer: time **plunge start** relative to Sweet & Clean (~1:50).
3. Both Prism: **orientation**, **pressure**, **stop at hiss**.

### Syphon

1. Log **heat level** (low/medium) and **drawdown duration**.
2. Stable + Bite: define **t=0** for 20 s and 40–45 s swirls.

### Moka

1. **Stronger:** run full workflow mirroring baseline; record **yield**, **shutdown cue**, **basket vs water level** at 200 g and 220 g.
2. Baseline: confirm **basket touches water** at 220 g if relevant to your machine.

## Additional fields worth adding (by method)

Suggestions only — add when you have data.

| Method | Optional fields |
|--------|-----------------|
| **V60** | Rinse filter; pre-wet; pulse vs continuous pour; final bed photo note; TDS if measured |
| **V60 Switch** | Pre-wet closed vs open; stir count during immersion; bypass water after release |
| **Aeropress Prism** | Inverted vs upright; metal filter maintenance; vacuum break before plunge |
| **Aeropress Paper** | Double paper; rinse volume; channeling check |
| **Syphon** | Cloth filter age / wash protocol; flame height; ambient temperature |
| **Moka** | Basket model; gasket state; preheat top chamber; cooling vessel; post-brew weight |

## Suggested fields from spec examples (not in recipes — do not add until tested)

The spec lists example historical notes (26 vs 25 clicks, thinner after cooling, 220 g vs valve). **None were added** unless already in repository content.
