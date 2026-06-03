# Contributing

This repository is documentation only — no build tools or apps.

**Language:** All recipe text, filenames, and docs should be in **English**.

**Guidelines:** Follow [docs/coffee-recipe-guidelines.md](docs/coffee-recipe-guidelines.md) and the method template in [docs/coffee-recipe-template-spec.md](docs/coffee-recipe-template-spec.md).

Every recipe should include **Evidence** (sources + confidence: High / Medium / Low) when values are reconstructed from other files or history.

## Adding or updating a recipe

1. Copy the **method-specific** template from `templates/`:

   | Folder | Template |
   |--------|----------|
   | `v60/` | `templates/v60-template.md` |
   | `v60-switch/` | `templates/v60-switch-template.md` |
   | `aeropress-prism/` | `templates/aeropress-prism-template.md` |
   | `aeropress-paper/` | `templates/aeropress-paper-template.md` |
   | `syphon/` | `templates/syphon-template.md` |
   | `electric-moka-pot/` | `templates/electric-moka-pot-template.md` |

2. Use a **kebab-case** filename from the **cup profile** (e.g. `strong.md`, `sweet-clean.md`), not grinder clicks or pour counts.
3. Keep **one recipe per file** and **all sections** from that method’s template (same order, same headings).
4. Do **not** invent parameters or tasting results. Missing values → `unknown`.
5. **V60:** every pour row needs water added, total water, and timing when known.
6. Set **Status** in the `## Status` section: `baseline`, `tested`, `experimental`, or `archived`.
7. Update **README.md** recipe table and **Related Recipes** links where useful.

## Folder layout

```
recipes/<coffee-name>/<method>/
```

Example: `recipes/robusta-honey/v60/strong.md`

## Style

- Short and practical — easy to tweak while brewing.
- Use English throughout.
- Put repeatability notes and use cases in **Historical Notes** or **Future Experiments** when they are not tasting results.
