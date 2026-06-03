# Recipe audit report

Audit date: 2026-06-03  
Guidelines: [coffee-recipe-guidelines.md](./coffee-recipe-guidelines.md)  
Templates: [coffee-recipe-template-spec.md](./coffee-recipe-template-spec.md)

Primary source: **Robusta Honey Recipes Source of Truth** (user-provided full recipe list, 2026-06-03). Prior placeholder V60 entries (`...` only) were replaced from this source.

---

## Summary

| Metric | Count |
|--------|------:|
| Recipes reviewed | 12 |
| Tested / baseline | 11 |
| Experimental (incomplete source) | 1 |
| Duplicates removed (historical) | 8 V60 files → 4 profiles |
| High overall confidence | 10 |
| Medium overall confidence | 2 |
| Low overall confidence | 1 |

---

## Recipes reviewed

| File | Method | Status | Overall confidence |
|------|--------|--------|-------------------|
| `v60/strong.md` | V60 | tested | **High** |
| `v60/balanced.md` | V60 | tested | **High** / **Medium** (200 g pour gap) |
| `v60/stable.md` | V60 | baseline | **High** |
| `v60/sweetness-body.md` | V60 | tested | **High** / **Medium** (limited Result detail) |
| `v60-switch/immersion-sweetness-body.md` | V60 Switch | tested | **High** |
| `syphon/sweet.md` | Syphon | tested | **High** |
| `syphon/stable-bite.md` | Syphon | tested | **High** (Medium for timer t=0) |
| `aeropress-prism/sweet-clean.md` | Aeropress Prism | tested | **High** |
| `aeropress-prism/killer.md` | Aeropress Prism | tested | **High** relative / **Low** absolute timing |
| `aeropress-paper/paper-filter.md` | Aeropress paper | tested | **High** workflow / **Low** press duration |
| `electric-moka-pot/current-baseline.md` | Moka | baseline | **High** |
| `electric-moka-pot/stronger-concentrated.md` | Moka | experimental | **High** params / **Low** workflow |

---

## Source-of-truth mapping

| Source ID | Repository file |
|-----------|-----------------|
| V60 #1 — Mocna, 3 zalania | `v60/strong.md` |
| V60 #2 — 24 kliki | `v60/balanced.md` |
| V60 #3 — 25 klików, 5 zalań | `v60/stable.md` |
| V60 #4 — 24 kliki, 190 g | `v60/sweetness-body.md` |
| V60 Switch #1 | `v60-switch/immersion-sweetness-body.md` |
| Syphon #1 — Słodka | `syphon/sweet.md` |
| Syphon #2 — Stabilna + Pazur | `syphon/stable-bite.md` |
| Aeropress Prism #1 | `aeropress-prism/sweet-clean.md` |
| Aeropress Prism #2 | `aeropress-prism/killer.md` |
| Aeropress Paper #1 | `aeropress-paper/paper-filter.md` |
| Electric Moka Pot #1 | `electric-moka-pot/current-baseline.md` |
| Electric Moka Pot #2 | `electric-moka-pot/stronger-concentrated.md` |

---

## Missing information (by recipe)

### V60 — Strong, Stable, Sweetness + body

Complete dose, water, temperature, grind, pour grams, cumulative totals, and timing where provided in source.

Still not in source:

- Pour start/end times per stage
- Pouring technique (style, swirl, flow)
- Drawdown duration
- Several Result subfields where source gave summary only

### V60 — Balanced

- Bloom time
- Total brew time
- Pouring technique
- Fourth pour or other step to reach **200 g** (listed pours sum to **165 g** after 30 g bloom)
- Several Result subfields except complexity / body trade-off

### V60 Switch

- Agitation, filter type
- Bitterness, clarity, strength, aftertaste, taste after cooling
- Exact drawdown split (derived as Medium)

### Aeropress Prism — Killer

- Exact plunge start (longer than Sweet & Clean’s 1:50), plunge duration, total brew time
- Setup: orientation, rinse, preheat
- Source gives relative extraction only: longer than Sweet & Clean, press slowly

### Aeropress — Paper filter

- Water temperature
- Number of filters; plunge duration; total time; sweetness in Result

### Syphon — both

- Water temperature; heat levels; drawdown duration
- Several Result subfields (body on Sweet, clarity on Stable + bite, etc.)

### Moka — stronger

- Entire workflow, shutoff, yield, water start (only params + Result in source)

### Moka — baseline

- Basket touches water; valve level; several Result subfields; cycle time

---

## Reconstructed information

| Recipe | Field | Value | Source | Confidence |
|--------|-------|-------|--------|------------|
| V60 Switch | Main pour 150 g | 190 − 40 bloom | Arithmetic from source | **High** |
| V60 Switch | Immersion 0:45–1:45 | 60 s closed | Bloom end + “hold to 1:45” | **Medium** |
| V60 Switch | Drawdown ~45–65 s | Within 2:30–2:50 total | Derived | **Medium** |
| V60 Balanced | Cumulative 75 / 120 / 165 g | Bloom 30 + three × 45 g | Arithmetic | **High** |
| Killer | Pressure light–medium | “press slowly” | Inferred | **Low** |
| All | Bean Robusta Honey, Comandante | Repository convention | All recipes | **High** |
| Syphon Sweet | Cloth filter | *filtr materiałowy* | Source | **High** |

**Not reconstructed (would be invention):** V60 Balanced pour to complete 200 g; syphon heat levels; paper water temperature; killer absolute plunge clock time; stronger moka workflow.

---

## Confidence levels (detail)

### High

Recipes with complete parameters + workflow + Result from source (or pour tables fully specified):

- All four V60 cards (except Balanced 200 g gap — see Medium)
- V60 Switch immersion
- Syphon Sweet and Stable + bite (except timer reference detail)
- Aeropress Sweet & Clean
- Moka current baseline

### Medium

- V60 Balanced: listed pours sum to 165 g vs 200 g target
- V60 sweetness-body: limited sensory Result beyond “more concentrated”
- V60 Switch: derived timing splits
- Syphon Stable + bite: t=0 for 20 s / 40–45 s swirls

### Low

- Moka stronger: workflow/shutoff/yield absent in source
- Killer / paper: absolute press durations where source omitted

---

## Duplicate recipes

Eight V60 files were consolidated into four profile-based files (no content loss — duplicates had no extra parameters):

| Removed (duplicate) | Canonical file |
|---------------------|----------------|
| `mocna-3-zalania.md`, `mocna-trzy-zalania.md` | `v60/strong.md` |
| `24-kliki.md`, `podstawowy-pour-over.md` | `v60/balanced.md` |
| `25-klikow-5-zalan.md`, `piec-zalan.md` | `v60/stable.md` |
| `24-kliki-190-g.md`, `woda-jak-switch.md` | `v60/sweetness-body.md` |

No duplicate active files remain.

---

## Inconsistent recipes

| Issue | Recipes | Notes |
|-------|---------|-------|
| V60 Balanced pour sum vs water target | balanced | 30 + 45×3 = 165 g documented; 200 g in Parameters — source gap, not repo conflict |
| Moka baseline water | baseline | Source: **220 g**; earlier repo had 200 g — corrected to source |
| Same grind, different method outcomes | V60 24 clicks vs Switch 24–25 | Documented separately; Switch tested for sweetness/body |
| Same ratio, different filters | Prism vs paper at 15 g / 150 g / 18 clicks | Documented A/B in Result — consistent |
| “Stable” naming | V60 stable vs Syphon stable-bite | Different methods; links clarify |
| Timer ambiguity | Switch 1:45; Syphon 20 s / 40–45 s | Marked Medium confidence |

No contradictory numeric parameters among fully specified recipes.

---

## Template compliance

| Requirement | Status |
|-------------|--------|
| Method-specific template per recipe | Yes — all 12 |
| Evidence section | Yes — all 12 |
| Tuning guide | Yes — all 12 |
| Warning signs | Yes — all 12 |
| Related recipes | Yes — all 12 |
| V60 complete pour tables | Yes — grams and cumulative totals from source |
| Aeropress extraction timelines | Yes — tested recipes |
| Syphon full workflow | Yes — numbered workflow + tables |
| Moka shutoff + yield | Yes — baseline; stronger partial |

---

## Recommendations for future experiments

### Priority 1 — V60 Balanced

1. Log how the cup reaches **200 g** (fourth pour or adjusted volumes).
2. Record bloom time and total brew time.

### Priority 2 — Moka stronger

1. Run full workflow; record yield, shutoff cue, and hot vs cold water start at 200 g / 18 clicks.

### Priority 3 — Timing clarity

1. V60 Switch: confirm 1:45 reference (brew start vs valve close).
2. Syphon Stable + bite: define t=0 for 20 s and 40–45 s.
3. Killer: measure plunge start vs Sweet & Clean (1:50).
4. Paper: measure temperature and exact plunge window after ~2 min.

### Priority 4 — Optional logging

- Taste after cooling (all methods).
- Syphon heat level and drawdown duration.
- V60 pour start/end times per stage.

---

## Files updated in this audit

- All 12 files under `recipes/robusta-honey/`
- [README.md](../README.md) — recipe index statuses
- This report: `docs/recipe-audit-report.md`

## Files not modified

- `templates/*`
- `docs/coffee-recipe-guidelines.md`, `docs/coffee-recipe-template-spec.md`, `docs/template-compliance-report.md`
