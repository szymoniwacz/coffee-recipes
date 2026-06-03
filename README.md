# coffee-recipes

Short coffee recipes in Markdown — one file per recipe, easy to edit, index below. Each card uses a **method-specific structure** (pour-over, Switch valve, press, syphon, moka).

Contributing: [CONTRIBUTING.md](CONTRIBUTING.md)
Guidelines: [docs/coffee-recipe-guidelines.md](docs/coffee-recipe-guidelines.md)
Template spec: [docs/coffee-recipe-template-spec.md](docs/coffee-recipe-template-spec.md)
Template compliance: [docs/template-compliance-report.md](docs/template-compliance-report.md)
Recipe audit: [docs/recipe-audit-report.md](docs/recipe-audit-report.md)

## Recipe Templates

Each method has its own template because different variables drive extraction and repeatability.

| Method | Template | Why separate? |
|--------|----------|---------------|
| V60 | [templates/v60-template.md](templates/v60-template.md) | Exact water per pour, bloom, and drawdown matter most. |
| V60 Switch | [templates/v60-switch-template.md](templates/v60-switch-template.md) | Valve state, immersion, and release timing matter most. |
| Aeropress Prism | [templates/aeropress-prism-template.md](templates/aeropress-prism-template.md) | Prism changes pressure, oils, and body. |
| Aeropress Paper | [templates/aeropress-paper-template.md](templates/aeropress-paper-template.md) | Paper filtration changes clarity and body vs Prism. |
| Syphon | [templates/syphon-template.md](templates/syphon-template.md) | Heat, upper-chamber timing, swirl, and drawdown matter most. |
| Electric moka pot | [templates/electric-moka-pot-template.md](templates/electric-moka-pot-template.md) | Water level, basket contact, shutoff cue, and yield matter most. |

## Recipes

| Method | Recipe | Coffee | Status | File |
|--------|--------|--------|--------|------|
| V60 | Strong | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/v60/strong.md](recipes/robusta-honey/v60/strong.md) |
| V60 | Balanced | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/v60/balanced.md](recipes/robusta-honey/v60/balanced.md) |
| V60 | Stable | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | baseline | [recipes/robusta-honey/v60/stable.md](recipes/robusta-honey/v60/stable.md) |
| V60 | Sweetness + body | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/v60/sweetness-body.md](recipes/robusta-honey/v60/sweetness-body.md) |
| V60 Switch | Immersion, sweetness + body | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/v60-switch/immersion-sweetness-body.md](recipes/robusta-honey/v60-switch/immersion-sweetness-body.md) |
| Syphon 3-cup | Sweet | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/syphon/sweet.md](recipes/robusta-honey/syphon/sweet.md) |
| Syphon 3-cup | Stable + bite | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/syphon/stable-bite.md](recipes/robusta-honey/syphon/stable-bite.md) |
| Aeropress Prism | Sweet & Clean | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/aeropress-prism/sweet-clean.md](recipes/robusta-honey/aeropress-prism/sweet-clean.md) |
| Aeropress Prism | Killer | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/aeropress-prism/killer.md](recipes/robusta-honey/aeropress-prism/killer.md) |
| Aeropress | Paper filter | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | tested | [recipes/robusta-honey/aeropress-paper/paper-filter.md](recipes/robusta-honey/aeropress-paper/paper-filter.md) |
| Electric moka pot | Current baseline | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | baseline | [recipes/robusta-honey/electric-moka-pot/current-baseline.md](recipes/robusta-honey/electric-moka-pot/current-baseline.md) |
| Electric moka pot | Stronger, more concentrated | Xin Chao Hanoi (100% Robusta, speciality) · 1996 Coffee | experimental | [recipes/robusta-honey/electric-moka-pot/stronger-concentrated.md](recipes/robusta-honey/electric-moka-pot/stronger-concentrated.md) |

## Structure

```
coffee-recipes/
├── README.md
├── CONTRIBUTING.md
├── docs/
│   ├── coffee-recipe-guidelines.md
│   ├── coffee-recipe-template-spec.md
│   ├── template-compliance-report.md
│   └── recipe-audit-report.md
├── templates/
│   ├── v60-template.md
│   ├── v60-switch-template.md
│   ├── aeropress-prism-template.md
│   ├── aeropress-paper-template.md
│   ├── syphon-template.md
│   └── electric-moka-pot-template.md
└── recipes/
    └── robusta-honey/
        ├── v60/
        ├── v60-switch/
        ├── syphon/
        ├── aeropress-prism/
        ├── aeropress-paper/
        └── electric-moka-pot/
```
