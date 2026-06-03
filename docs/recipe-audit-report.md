# Recipe audit report

Audit date: 2026-06-03  
Guidelines: [coffee-recipe-guidelines.md](./coffee-recipe-guidelines.md)  
Templates: [coffee-recipe-template-spec.md](./coffee-recipe-template-spec.md)

## Summary

| Metric | Count |
|--------|------:|
| Recipes reviewed | 12 |
| Tested / baseline | 8 |
| Experimental (incomplete source) | 4 |
| Duplicates removed (historical) | 8 V60 files → 4 profiles |
| High overall confidence | 7 |
| Medium overall confidence | 2 |
| Low overall confidence | 3 |

Primary source for tested recipes: initial user recipe paste (preserved in conversation transcript). Secondary: current recipe files, [template-compliance-report.md](./template-compliance-report.md), cross-links between recipes. **No git history** of recipe bodies (only templates in commit `88a81f7`).

---

## Recipes reviewed

| File | Method | Status | Overall confidence |
|------|--------|--------|-------------------|
| `v60-switch/immersion-sweetness-body.md` | V60 Switch | tested | **High** |
| `syphon/sweet.md` | Syphon | tested | **High** |
| `syphon/stable-bite.md` | Syphon | tested | **High** (Medium for timer t=0) |
| `aeropress-prism/sweet-clean.md` | Aeropress Prism | tested | **High** |
| `aeropress-prism/killer.md` | Aeropress Prism | tested | **High** relative / **Low** absolute timing |
| `aeropress-paper/paper-filter.md` | Aeropress paper | tested | **High** workflow / **Low** press duration |
| `electric-moka-pot/current-baseline.md` | Moka | baseline | **High** |
| `electric-moka-pot/stronger-concentrated.md` | Moka | experimental | **High** params / **Low** workflow |
| `v60/strong.md` | V60 | experimental | **Low** |
| `v60/balanced.md` | V60 | experimental | **Low** |
| `v60/stable.md` | V60 | experimental | **Low** |
| `v60/sweetness-body.md` | V60 | experimental | **Medium** (water/grind) / **Low** cup |

---

## Missing information (by recipe)

### V60 — all four

| Field | strong | balanced | stable | sweetness-body |
|-------|--------|----------|--------|----------------|
| Dose | missing | missing | missing | 15 g (Medium — A/B intent) |
| Water total | missing | missing | missing | **190 g** |
| Grind | missing | **24 clicks** | **25 clicks** | **24 clicks** |
| Pour count | **3** | not in source | **5** | not in source |
| Pour grams/times | all missing | all missing | all missing | all missing |
| Temperature, Result | missing | missing | missing | missing (goal from Switch) |

**Root cause:** Original paste used `...` for V60 #1–#4 with titles only.

### V60 Switch

- Agitation, filter type, origin/process/roast
- Bitterness, clarity, strength, aftertaste, taste after cooling
- Exact drawdown split (derived as Medium)

### Aeropress Prism — Killer

- Exact plunge start (after 1:50), plunge duration, total brew time
- Setup: orientation, rinse, preheat

### Aeropress — Paper filter

- Water temperature
- Number of filters; plunge duration; total time; sweetness in Result

### Syphon — both

- Water temperature; heat levels; drawdown duration
- Several Result subfields (body on Sweet, clarity on Stable + bite, etc.)

### Moka — stronger

- Entire workflow, shutoff, yield (only params + Result in source)
- Water start (hot assumed Low confidence from baseline mirror)

### Moka — baseline

- Basket touches water; valve level; several Result subfields; cycle time

---

## Reconstructed information

| Recipe | Field | Value | Source | Confidence |
|--------|-------|-------|--------|------------|
| V60 Switch | Main pour 150 g | 190 − 40 bloom | Arithmetic from source | **High** |
| V60 Switch | Immersion 0:45–1:45 | 60 s closed | Bloom end + “hold to 1:45” | **Medium** |
| V60 Switch | Drawdown ~45–65 s | Within 2:30–2:50 total | Derived | **Medium** |
| sweetness-body | Dose 15 g, ratio 1:12.7 | Switch A/B + filename | Cross-recipe | **Medium** |
| stronger-concentrated | Workflow steps 1–6 | Mirror baseline | Hypothesis for next test | **Low** |
| Killer | Pressure light–medium | “press slowly” | Inferred | **Low** |
| All | Bean Robusta Honey, Comandante | Repository convention | All recipes | **High** |
| Syphon | Cloth filter | *filtr materiałowy* | Source | **High** |

**Not reconstructed (would be invention):** V60 pour grams per stage, V60 temperatures, syphon heat levels, paper water temperature, killer absolute plunge clock time.

---

## Confidence levels (detail)

### High

Recipes with complete parameters + workflow + Result from source:

- V60 Switch immersion
- Syphon Sweet and Stable + bite (except timer reference detail)
- Aeropress Sweet & Clean
- Moka current baseline

### Medium

- V60 sweetness-body: 190 g, 24 clicks, 15 g dose intent
- V60 Switch: derived timing splits
- Syphon Stable + bite: t=0 for 20 s / 40–45 s swirls

### Low

- All four V60 pour-over cards (except partial metadata above)
- Moka stronger workflow/shutoff/yield
- Killer / paper absolute press durations where source omitted

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
| Same grind, different method outcomes | V60 24 clicks vs Switch 24–25 vs sweetness-body | Switch tested; V60 not — do not equate cups |
| Same ratio, different filters | Prism vs paper at 15 g / 150 g / 18 clicks | Documented A/B in Result — consistent |
| “Stable” naming | V60 stable vs Syphon stable-bite | Different methods; links clarify |
| Timer ambiguity | Switch 1:45; Syphon 20 s / 40–45 s | Marked Medium confidence; needs one clarifying brew |
| Stronger moka workflow | baseline vs stronger | Stronger missing source workflow — Low confidence mirror |

No contradictory numeric parameters found among tested recipes.

---

## Template compliance

| Requirement | Status |
|-------------|--------|
| Method-specific template per recipe | Yes — all 12 |
| Evidence section | Yes — all 12 |
| Tuning guide | Yes — all 12 |
| Warning signs | Yes — all 12 |
| Related recipes | Yes — all 12 |
| V60 complete pour tables | Yes — structure complete; grams/times **not documented** where source omitted |
| Aeropress extraction timelines | Yes — tested recipes |
| Syphon full workflow | Yes — numbered workflow + tables |
| Moka shutoff + yield | Yes — baseline; stronger partial |

---

## Recommendations for future experiments

### Priority 1 — V60 line

1. Brew **sweetness-body** at 15 g / 190 g / 24 clicks; log every pour to 190 g and full Result.
2. Brew **balanced**, **stable**, **strong** with logged dose, water, temperature, and pour tables.
3. Compare V60 sweetness-body vs Switch at same dose and water.

### Priority 2 — Moka stronger

1. Run full workflow mirroring baseline with 200 g / 18 clicks.
2. Record yield, shutoff cue, and basket–water level at 200 g vs 220 g.

### Priority 3 — Timing clarity

1. V60 Switch: confirm 1:45 reference (brew start vs valve close).
2. Syphon Stable + bite: define t=0 for 20 s and 40–45 s.
3. Killer: measure plunge start vs Sweet & Clean (1:50).
4. Paper: measure temperature and exact plunge window after 2:00.

### Priority 4 — Optional logging

- Taste after cooling (all methods).
- Syphon heat level and drawdown duration.
- Aeropress orientation, filter rinse, stop at hiss.

---

## Files updated in this audit

- All 12 files under `recipes/robusta-honey/`
- This report: `docs/recipe-audit-report.md`

## Files not modified

- `templates/*` (unchanged; recipes add Evidence beyond template stubs)
- `docs/coffee-recipe-guidelines.md`, `docs/coffee-recipe-template-spec.md` (source of truth)
