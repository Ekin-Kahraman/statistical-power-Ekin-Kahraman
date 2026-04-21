# Statistical Power — 5023B Session 3

Simulation-based power analysis workshop submission.

## Structure

- `session3_assessment.qmd` — the assessment document. Renders to a
  self-contained HTML that is the submission to Blackboard.
- `data/` — any CSVs used by the analysis (referenced with relative paths).

## Render

```bash
quarto render session3_assessment.qmd
```

Or in RStudio: open the .qmd and click **Render**.

## Commitment summary

- Effect size: 0.80 g (Option 3 — minimum meaningful difference at Wytham Woods)
- Residual SD: 2.10 g (Option 3 — 15-year tarsus-adjusted Wytham data)
- Model: `lm(body_mass ~ treatment + tarsus_length)`
- 1000 simulations per (n, effect, sigma) cell, α = 0.05

## Packages

`tidyverse`, `broom`, `ggdag`, `dagitty`.
