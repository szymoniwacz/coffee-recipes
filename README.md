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
