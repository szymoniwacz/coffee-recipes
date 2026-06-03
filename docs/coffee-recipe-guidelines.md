# Coffee Recipes Repository Guidelines

## Purpose

This repository is a long-term coffee knowledge base.
It is not just a collection of recipes.

Every recipe should document:
- Exact brewing parameters
- Brewing workflow
- Observed results
- Historical context
- Tuning guidance
- Repeatability information

---

# General Rules

## One recipe per file

Each recipe must live in its own Markdown file.

Examples:

- recipes/robusta-honey/v60/sweetness-body.md
- recipes/robusta-honey/syphon/sweet.md
- recipes/robusta-honey/electric-moka-pot/current-baseline.md

## Do not lose information

Never remove historical notes.
Never replace known information with "unknown".

If information exists elsewhere in the repository:
- recipe notes
- archived files
- git history
- README
- migration reports

then reconstruct the recipe.

---

# Reconstruction Rules

When updating recipes:

1. Search the entire repository.
2. Reconstruct missing values from evidence.
3. Merge knowledge from previous versions.
4. Record assumptions.

Example:

If:
- filename contains "25-clicks-5-pours"
- another document contains full parameters

then use those parameters.

Do not leave fields as unknown if evidence exists.

---

# Method-Specific Templates

## V60

Must contain:

### Coffee
- Bean
- Origin
- Process
- Roast level
- Roaster

### Equipment
- Brewer
- Filter
- Grinder
- Kettle
- Scale

### Parameters
- Coffee dose
- Water amount
- Brew ratio
- Water temperature
- Grind size
- Water type

### Pour Structure

Required table:

| Stage | Water Added | Total Water | Start Time | End Time | Notes |
|---------|---------:|---------:|---------|---------|---------|

Every pour must be recorded.

Examples:
- Bloom
- Pour #1
- Pour #2
- Pour #3
- Pour #4

### Pouring Technique

- Pour style
- Agitation
- Swirl
- Stirring
- Flow rate

### Timing

- Bloom time
- Drawdown time
- Total brew time

### Result

- Sweetness
- Body
- Acidity
- Bitterness
- Clarity
- Strength
- Aftertaste
- Taste after cooling

### Extraction Logic

Explain:
- grind choice
- temperature choice
- pour structure

### Tuning Guide

| Goal | Change |
|--------|--------|

### Warning Signs

| Symptom | Cause | Adjustment |
|--------|--------|--------|

### Historical Notes

### Related Recipes

### Future Experiments

---

## V60 Switch

Everything from V60 plus:

### Switch Parameters

- Immersion style
- Valve state
- Bloom style
- Immersion time
- Release moment
- Drawdown behavior

Document:
- when valve is opened
- why it is opened there

---

## Aeropress Prism

### Parameters

- Coffee dose
- Water amount
- Ratio
- Temperature
- Grind size

### Setup

- Prism installed
- Orientation
- Filter details

### Workflow

- Bloom
- Stirring
- Swirl
- Steep time
- Plunge start
- Plunge duration

### Pressure

- Light
- Medium
- Heavy

### Result

### Extraction Logic

### Tuning Guide

### Historical Notes

---

## Aeropress Paper

Everything from Aeropress plus:

### Filter

- Paper type
- Rinsed or not
- Number of filters

### Setup

- Upright / inverted

Document expected differences versus Prism.

---

## Syphon

### Equipment

- Filter type
- Burner
- Brewer size

### Workflow

- When upper chamber attached
- When coffee added
- Stirring pattern
- Swirl pattern
- Contact time
- Heat removal timing
- Drawdown observations

### Result

### Extraction Logic

### Tuning Guide

### Historical Notes

Special attention:
Material filter observations should be preserved.

---

## Electric Moka Pot

### Parameters

- Coffee dose
- Water amount
- Ratio
- Grind size

### Water

- Hot or cold start
- Basket touching water or not

### Preparation

- Fill method
- Leveling
- Tamping

### Brew

- Start conditions
- First drops
- Stream behavior
- Shutdown cue

### Yield

- Final beverage weight

### Warning Signs

- Overheating
- Late shutdown
- Burnt notes
- Weak extraction

### Result

### Historical Notes

---

# Confidence Levels

Every reconstructed recipe should contain:

## Evidence

- Source files
- Historical notes used

Confidence:

- High
- Medium
- Low

---

# Naming Rules

Use human-readable names.

Good:

- sweetness-body.md
- sweet-clean.md
- stable-bite.md

Avoid:

- recipe-01.md
- v60-test-4.md

---

# Repository Goal

The repository should answer:

- What recipe was used?
- Why was it created?
- What happened?
- How can it be improved?
- Which recipe is better for a specific goal?

A future reader should be able to reproduce every successful recipe without reading commit history or old notes.
