---
layout: case-study
title: Quantitative Methods
description: How I use statistics to pressure-test research claims, product feedback, and design guidance
meta:
  role: Researcher and analyst
  duration: 2020 - 2026
  company: Academic and applied research work
  tools: R, NPS, qualtRics, likert, sentimentr, lme4, MuMIn, LPA
---

# Quantitative Methods

I do not think of quantitative methods as a separate credential box. They are the part of the work where I slow down and ask: **what would make this interpretation wrong, too strong, or not useful enough?**

That shows up in a few recurring places: experimental analysis, NPS and product-feedback decomposition, response-quality decisions, segmentation, and nested data. The details change by project, but the habit is the same: make the statistical claim specific enough that it can be checked.

## Experimental Validation

For the dashboard knowledge-retention dissertation, the statistical work was not just "run the ANOVA and report the p-value." The point was to make the design claim harder to knock over.

I checked the main results several ways:

- Robust and nonparametric checks for bounded quiz-score data
- Bootstrap confidence intervals for effect sizes
- Planned contrasts for the hierarchy comparisons that mattered theoretically
- Equivalence tests for chartjunk effects that were statistically detectable but not very useful
- Sensitivity power analysis for the observed hierarchy effects

The useful takeaway stayed simple: hierarchy alignment carried the design argument. Chartjunk did not. The extra checks mattered because they kept that sentence from becoming cleaner than the evidence.

<div class="image-gallery single">
<div>
<img src="{{ '/assets/images/portfolio/quantitative-methods/contrasts.png' | relative_url }}" alt="Planned contrast results for dashboard hierarchy conditions">
<div class="caption">Planned contrasts made the hierarchy finding easier to interpret than an omnibus test alone.</div>
</div>
</div>

## Response Quality And Sensitivity Workflows

Online studies are easy to run and easy to fool yourself with. I keep response-quality work close to the analysis instead of treating it as housekeeping.

I also maintain a public teaching vignette for careless-responding workflows. It uses synthetic data, so the method can be shared without exposing participant records, but it still behaves like a realistic online experiment pipeline.

The workflow is built around defensible screening, not result-shopping:

- Attention checks and duration flags
- Longstring and within-person variability checks for Likert batteries
- Sensitivity analysis comparing raw and screened estimates
- Methods language that records the rule before interpreting the model

That last part is important. If the screening rule only becomes clear after the results are known, it is no longer just quality control.

## NPS And Product Feedback Decomposition

NPS is useful as a smoke alarm, not as an explanation. A top-line score can tell a team that something changed, but it does not say whether the change came from a product capability, support expectation, documentation gap, regional pattern, or one loud category of open-text feedback.

The R workflow I used decomposed product-feedback surveys into those more usable pieces:

- `qualtRics` for pulling survey waves directly from Qualtrics rather than treating exports as one-off spreadsheets
- `NPS` for score calculation and wave-to-wave NPS tests
- `likert` for decomposing adjacent satisfaction and capability items by survey wave
- `ggplot2` and `ggthemes` for readable comparisons that stakeholders could scan quickly
- `readr`, `readxl`, and `reshape2` for moving between CSV/Excel exports and long-form analysis tables
- `sentimentr` for category-level summaries of open-text feedback
- `choroplethr`, `choroplethrMaps`, and `rgeolocate` for checking whether responses were geographically concentrated

The practical move was to refuse the easy ending of "NPS went up" or "NPS went down." I wanted to know which part of the experience had moved, whether the movement also showed up in satisfaction items, and whether open-text comments told the same story.

## Segmentation And Persona Modeling

Latent profile analysis was useful in my persona work because it put friction in the right place. Instead of deciding the segments first and then finding quotes to decorate them, the model forced the team to start with response patterns.

I still do not treat a profile solution as finished because the fit indices look good. A useful segmentation has to survive three questions:

- Do the groups separate cleanly enough to matter?
- Can a researcher explain the difference without laundering noise into story?
- Do interviews with people in those groups make the segments more real, not less?

That is the version of quant work I trust: numbers strong enough to challenge assumptions, and qualitative follow-up strong enough to keep the numbers human.

The public persona page covers this work in more detail: [Healthcare Persona Development]({{ '/portfolio/persona/' | relative_url }}).

## GLMM Work In R

Some questions are nested whether the report admits it or not: people inside groups, repeated responses inside people, observations inside time periods or contexts. For multilevel and generalized linear mixed-model work, I use results-free public examples when the applied data cannot be shared.

The inspectable R pattern uses:

- `lme4` for random-intercept, random-slope, and three-level model structures
- `lmerTest` when the model needs inferential tests around fixed effects
- `MuMIn::r.squaredGLMM()` for marginal and conditional variance explained
- `sjPlot::tab_model()` for turning model output into a reviewable table
- `tidyverse`, `dplyr`, and `ggplot2` for data shaping, predictions, and model-check plots

The method decisions matter more than the package names: what the outcome distribution allows, which grouping structure belongs in the model, whether a random slope is doing real work, and how much variance lives in the fixed effects versus the grouped structure.

That boundary is deliberate. The method can be inspected without pretending confidential applied results belong on a public portfolio page.

## Why This Matters

The through-line is not a single technique. It is a working habit: choose the model that matches the question, run checks that could puncture the easy story, and translate the result into language a research or product audience can actually use.
