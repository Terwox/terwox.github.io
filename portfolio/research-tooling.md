---
layout: case-study
title: Research Tooling
description: Public-safe examples of research operations, reproducible reporting, and AI-assisted validation systems
meta:
  role: Research systems designer
  duration: 2021 - 2026
  company: Academic and applied research portfolio
  tools: R, Python, Qualtrics, UserZoom, Jinja2, Plotly, Quarto, LLM review pipelines
---

# Research Tooling

My research work often sits between study design and production workflow: building the tools that make research reproducible, reviewable, and safe to share.

## Online Experimentation Instrumentation

The dissertation studies and response-quality teaching materials use modern online research instrumentation:

- Qualtrics and UserZoom workflows for timed exposure and randomized stimulus presentation.
- Dashboard stimuli with controlled design manipulations.
- Attention checks, domain checks, duration rules, and careless-responding metrics.
- Reproducible R and Python pipelines for cleaning, analysis, and reporting.

The goal is not just to collect data. It is to make the data-collection system auditable enough that another researcher can understand how exclusions, scoring, and analysis decisions were made.

## Reproducible Reporting Pipelines

I have also built reporting systems that turn structured feedback into self-contained HTML deliverables. The public-safe architecture pattern is:

- **Configuration over code:** thresholds, colors, column names, windows, and weights live in config or YAML.
- **Synthetic-data-first development:** the report can be built, tested, and demonstrated without touching real records.
- **Layered separation:** data transforms, chart builders, templates, and branding are swappable.
- **Self-contained output:** charts, fonts, icons, and sparklines ship in a single portable report.
- **Stable identifiers:** one issue slug or category key can connect icon lookup, rendered DOM elements, and temporal tracking.

This architecture makes a report useful beyond one dataset or one stakeholder request.

## Trustworthy AI-Assisted Synthesis

The most important LLM pattern I use is **fresh generation, adversarial review, then temporal reconciliation**.

The reporting workflow deliberately avoids feeding the previous narrative into the first draft. Instead, it generates a fresh report from current evidence, reviews it through multiple lenses, extracts factual assertions only after review, and then reconciles those assertions against prior periods.

That design prevents old hallucinations from being copied forward while still preserving continuity.

<div class="image-gallery single">
<div>
<img src="{{ '/assets/images/portfolio/research-tooling/workflow-preview.png' | relative_url }}" alt="Fresh generation, adversarial review, assertion extraction, and temporal reconciliation workflow">
<div class="caption">High-level public-safe architecture for trustworthy recurring research reports.</div>
</div>
</div>

### Hosted Artifacts

- [Workflow visualization]({{ '/portfolio/assets/voc-pipeline-workflow.html' | relative_url }})
- [Adversarial review prompt structure]({{ '/portfolio/assets/adversarial-review-prompts.html' | relative_url }})

## Practical Boundary

The examples here are intentionally public-safe. They describe architecture, method, and reusable design patterns without publishing row-level participant data, confidential verbatims, internal metrics, product names, or client-specific reports.
