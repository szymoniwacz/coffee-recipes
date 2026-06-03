# Coffee Recipe Template Specification

This file defines method-specific Markdown templates for the `coffee-recipes` repository.

Goal: create templates that match how each brewing method actually works. Do not force one generic template across all recipes.

Repository should remain Markdown-only.

---

# General Rules

## Folder

Create or update templates in:

```text
templates/
  v60-template.md
  v60-switch-template.md
  aeropress-prism-template.md
  aeropress-paper-template.md
  syphon-template.md
  electric-moka-pot-template.md
```

## Rules for all templates

- One recipe = one Markdown file.
- Preserve all existing recipe information.
- Do not invent missing details.
- If a field is unknown, write `unknown`.
- Use grams, Celsius, and Comandante clicks where possible.
- Always include brew ratio when coffee dose and water amount are known.
- Keep tasting notes structured and comparable.
- Keep historical notes. They are important.
- Add cross-links to related recipes where useful.
- Each method has its own variables, so each method needs its own template.

## Common sections used in all templates

Every template should include these shared sections:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment

## Parameters

## Workflow

## Timing

## Result

## Tuning Guide

## Warning Signs

## Historical Notes

## Related Recipes

## Future Experiments
```

---

# V60 Template

V60 recipes must precisely describe every pour. For Szymon's recipes this is the most important part.

File:

```text
templates/v60-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

Describe the purpose of this V60 recipe.

Examples:
- more sweetness
- more body
- stronger cup
- less acidity
- better taste after cooling

## Equipment
- Brewer: V60
- Filter:
- Grinder:
- Kettle:
- Scale:

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water temperature:
- Grind size:
- Water type:

## Pour Structure

Every V60 recipe must include exact water amount per pour and cumulative water total.

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom |  |  | 0:00 |  |  |
| Pour #1 |  |  |  |  |  |
| Pour #2 |  |  |  |  |  |
| Pour #3 |  |  |  |  |  |
| Pour #4 |  |  |  |  |  |
| Pour #5 |  |  |  |  |  |

Remove unused pour rows only if they do not apply.

## Pouring Technique
- Pour style:
- Center pour / circular pour:
- Agitation:
- Swirl:
- Stirring:
- Flow rate:
- Bed shape target:

## Timing
- Bloom time:
- Drawdown time:
- Total brew time:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain why the grind size, temperature, number of pours and pour amounts work for this recipe.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More strength |  |
| Less bitterness |  |
| Less acidity |  |
| Less watery taste |  |
| Better taste after cooling |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Watery / thin |  |  |
| Harsh bitterness |  |  |
| Sourness / acidity |  |  |
| Slow drawdown |  |  |
| Fast drawdown |  |  |

## Historical Notes

Record observed differences between V60 variants.

Examples:
- 25 clicks had more body than 26 clicks.
- 26 clicks became slightly diluted compared to 25.
- 24 clicks improved complexity but reduced body.
- Some variants became thinner after cooling.

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# V60 Switch Template

V60 Switch recipes must capture valve state, immersion time and release timing.

File:

```text
templates/v60-switch-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment
- Brewer: V60 Switch
- Filter:
- Grinder:
- Kettle:
- Scale:

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water temperature:
- Grind size:
- Water type:

## Brew Style
- Style: full immersion / hybrid / percolation-first / immersion-first
- Valve at start: open / closed
- Bloom: yes / no
- Bloom water:
- Bloom time:

## Water Schedule

| Stage | Valve state | Water added | Total water | Start time | End time | Notes |
|---|---|---:|---:|---|---|---|
| Bloom |  |  |  | 0:00 |  |  |
| Main pour |  |  |  |  |  |  |
| Release | open |  |  |  |  |  |

## Immersion And Release
- Immersion start:
- Immersion end:
- Valve open time:
- Drawdown time after release:
- Total brew time:

## Agitation
- Stirring:
- Swirl:
- Agitation before release:
- Bed settling notes:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain how closed-valve immersion, bloom, release time and grind size affect this recipe.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More clarity |  |
| More strength |  |
| Less bitterness |  |
| Less acidity |  |
| Faster drawdown |  |
| Slower extraction |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Watery / hollow |  |  |
| Muddy / heavy |  |  |
| Bitter / dry |  |  |
| Sour / sharp |  |  |
| Drawdown too slow |  |  |

## Historical Notes

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# Aeropress Prism Template

Aeropress Prism recipes must capture bloom, steep time, stirring and pressing style. Prism changes body and oils, so it should not use the same template as paper Aeropress.

File:

```text
templates/aeropress-prism-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment
- Brewer: Aeropress
- Attachment: Fellow Prismo / Prism
- Filter: metal / paper + metal / unknown
- Grinder:
- Kettle:
- Scale:

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water temperature:
- Grind size:
- Water type:
- Bypass: yes / no
- Bypass amount:

## Setup
- Orientation: upright / inverted
- Filter rinse: yes / no / not applicable
- Preheat brewer: yes / no / unknown

## Water And Bloom

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom |  |  | 0:00 |  |  |
| Main pour |  |  |  |  |  |
| Bypass |  |  |  |  | optional |

## Agitation
- Stirring count:
- Stirring style:
- Swirl:
- Agitation timing:

## Steep And Press
- Steep start:
- Plunge start:
- Plunge duration:
- Pressure level: light / medium / strong
- Stop at hiss: yes / no / unknown
- Total brew time:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Oiliness:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain why this recipe uses Prism, selected grind, steep time, agitation and pressure.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More strength |  |
| More clarity |  |
| Less bitterness |  |
| Less acidity |  |
| Less muddy cup |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Too intense / harsh |  |  |
| Too weak |  |  |
| Bitter / dry |  |  |
| Sour / thin |  |  |
| Hard to press |  |  |
| Too oily / muddy |  |  |

## Historical Notes

Record differences between Sweet & Clean and Killer variants.

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# Aeropress Paper Template

Paper Aeropress recipes need filter and clarity details. They should be separate from Prism recipes.

File:

```text
templates/aeropress-paper-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment
- Brewer: Aeropress
- Filter: paper
- Number of filters:
- Grinder:
- Kettle:
- Scale:

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water temperature:
- Grind size:
- Water type:
- Bypass: yes / no
- Bypass amount:

## Setup
- Orientation: upright / inverted
- Filter rinse: yes / no
- Preheat brewer: yes / no / unknown

## Water And Bloom

| Stage | Water added | Total water | Start time | End time | Notes |
|---|---:|---:|---|---|---|
| Bloom |  |  | 0:00 |  |  |
| Main pour |  |  |  |  |  |
| Bypass |  |  |  |  | optional |

## Agitation
- Stirring count:
- Stirring style:
- Swirl:
- Agitation timing:

## Steep And Press
- Steep start:
- Plunge start:
- Plunge duration:
- Pressure level: light / medium / strong
- Stop at hiss: yes / no / unknown
- Total brew time:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Cleanliness:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain how paper filtration, grind size, steep time and pressure affect clarity and body.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More clarity |  |
| More strength |  |
| Less bitterness |  |
| Less acidity |  |
| Less paper taste |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Too clean / thin |  |  |
| Too weak |  |  |
| Bitter / dry |  |  |
| Sour / thin |  |  |
| Hard to press |  |  |
| Paper taste |  |  |

## Historical Notes

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# Syphon Template

Syphon recipes need heat control, chamber timing, stirring and drawdown behavior.

File:

```text
templates/syphon-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment
- Brewer: syphon 3-cup
- Filter: cloth / paper / metal / unknown
- Heat source:
- Grinder:
- Scale:

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water temperature:
- Grind size:
- Water type:

## Setup
- Upper chamber attached from start: yes / no
- Filter type:
- Filter preparation:
- Water added to lower chamber:
- Preheating notes:

## Heat Control
- Initial heat level:
- Heat level after water rises:
- Heat adjustment during contact:
- Heat removed at:

## Coffee Addition And Contact
- Coffee added when:
- Contact start:
- Contact duration:
- Contact end:
- Total upper chamber time:

## Stirring / Swirl Pattern

| Time | Action | Intensity | Notes |
|---|---|---|---|
| Coffee added |  |  |  |
| 20 s |  |  |  |
| 40–45 s |  |  |  |
| Before drawdown |  |  |  |

## Drawdown
- Heat removed at:
- Drawdown start:
- Drawdown duration:
- Drawdown behavior:
- Final bed shape:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Aroma:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain how filter type, grind, contact time, heat and swirl pattern affect the cup.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More clarity |  |
| More strength |  |
| Less bitterness |  |
| Less acidity |  |
| Faster drawdown |  |
| More expressive cup |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Too clean / thin |  |  |
| Too heavy / muddy |  |  |
| Bitter / dry |  |  |
| Sour / sharp |  |  |
| Drawdown too slow |  |  |
| Weak aroma |  |  |

## Historical Notes

Record filter observations.

Examples:
- Cloth filter tasted better.
- Sweet variant had about 60 s contact.
- Stable + Pazur used shorter contact and stronger swirl pattern.

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# Electric Moka Pot Template

Electric moka pot recipes must capture water amount, basket-water contact, shutdown cue and yield. These matter more than exact timing because the device has limited temperature control.

File:

```text
templates/electric-moka-pot-template.md
```

Template content:

```md
# Recipe Name

## Status
- Status: baseline / tested / experimental / archived
- Last updated:

## Coffee
- Bean:
- Origin:
- Process:
- Roast level:

## Goal

## Equipment
- Brewer: electric moka pot
- Grinder:
- Scale:
- Heat control: fixed / one-button / unknown

## Parameters
- Coffee dose:
- Water amount:
- Brew ratio:
- Water start: hot / cold
- Grind size:
- Basket filled to:
- Basket touches water: yes / no / unknown

## Preparation
- Water amount in base:
- Water level relative to valve:
- Coffee dose in basket:
- Coffee distribution:
- Leveling:
- Tamping: no / light / yes
- Top chamber preheated: yes / no / unknown

## Brewing Workflow
1. 
2. 
3. 
4. 
5. 

## Shutdown Cue
- Shutdown cue:
- Stream color at shutdown:
- Bubbling at shutdown:
- Sound cue:
- Reason for shutdown timing:

## Yield
- Expected yield:
- Actual yield:
- Yield ratio:

## Result
- Sweetness:
- Body:
- Acidity:
- Bitterness:
- Clarity:
- Strength:
- Roast / burnt notes:
- Aftertaste:
- Taste after cooling:

## Extraction Logic

Explain how water amount, grind size, hot water start, shutdown cue and yield affect strength, body and overheating.

## Tuning Guide

| Goal | Change |
|---|---|
| More sweetness |  |
| More body |  |
| More strength |  |
| Less burnt taste |  |
| Less bitterness |  |
| Less watery taste |  |
| Higher yield |  |
| Lower yield / more concentration |  |

## Warning Signs

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Burnt / overheated |  |  |
| Watery / thin |  |  |
| Bitter / harsh |  |  |
| Weak / low body |  |  |
| Too little yield |  |  |
| Basket touches water |  |  |

## Historical Notes

Record observations from previous moka pot experiments.

Examples:
- 220 g water may reach the valve but can make the basket touch water in some setups.
- 200 g water fits under the valve better.
- Turning off before heavy bubbling reduced overheating.
- Turning off at stream lightening produced about 175 g yield.
- 18 clicks gave more concentration but less sweetness and a slightly burnt character.

## Related Recipes
- See also:

## Future Experiments
- 
```

---

# README Update Instructions

Update `README.md` to include a section:

```md
## Recipe Templates

Each brewing method has its own template because each method depends on different variables.

| Method | Template | Why separate? |
|---|---|---|
| V60 | templates/v60-template.md | Exact pour amounts and drawdown matter most. |
| V60 Switch | templates/v60-switch-template.md | Valve state, immersion and release timing matter most. |
| Aeropress Prism | templates/aeropress-prism-template.md | Prism changes pressure, oils and body. |
| Aeropress Paper | templates/aeropress-paper-template.md | Paper filtration changes clarity and body. |
| Syphon | templates/syphon-template.md | Heat, chamber timing, swirl and drawdown matter most. |
| Electric Moka Pot | templates/electric-moka-pot-template.md | Shutdown cue, water level and yield matter most. |
```

---

# Cursor Task

Use this file as the source of truth.

Tasks:

1. Create or replace all method-specific template files in `templates/`.
2. Update all existing recipe files so each recipe follows the correct template for its brewing method.
3. Preserve all current recipe details.
4. Do not invent missing information.
5. Use `unknown` for missing fields.
6. Update `README.md` with links to all templates.
7. Keep the repository Markdown-only.
8. Make the result easy to maintain manually.
