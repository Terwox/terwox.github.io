---
layout: case-study
title: Dashboard Knowledge Retention
description: Doctoral research on how dashboard organization affects what users remember
meta:
  role: Principal Researcher
  duration: 2012 - 2026
  company: University of South Dakota
  tools: R, Qualtrics, UserZoom, factorial experiments, mixed methods
---

# Dashboard Knowledge Retention

**Ph.D. completed April 2026** | Manuscript-ready findings and statistical validation complete

## The Problem

Dashboards are often treated as real-time monitoring surfaces, but users carry dashboard information into later decisions after the display is gone. My dissertation asked a practical human factors question: **which dashboard design choices help people retain what they saw?**

The project moved from formative design work into controlled experiments, using dashboard knowledge retention as the outcome instead of relying only on preference, speed, or self-reported usability.

## Research Program

The completed dissertation focused on three connected phases:

| Phase | Purpose | Evidence produced |
| --- | --- | --- |
| Formative work | Identify dashboard design factors worth testing | Expert review, heuristic analysis, and co-creation sessions pointed to visual hierarchy and chartjunk |
| IT dashboard experiment | Test hierarchy and chartjunk in an operational dashboard context | A 2x2 factorial experiment using a timed dashboard exposure and retention quiz |
| Smart home dashboard experiment | Replicate and extend the design manipulations in a more familiar domain | A 4x3 factorial experiment comparing importance, none, room, and floorplan hierarchies across chartjunk levels |

## Core Finding

The most useful design principle was not "remove decoration." It was **align spatial organization with the task users need to perform**.

Across the experimental studies, hierarchy affected retention more consistently than chartjunk. Importance-based organization helped when users needed to understand priority and severity. Room and floorplan layouts performed worse when the questions were not spatial, because the display structure pushed attention toward relationships that did not help the task.

## Methods

### Experimental Design

Participants viewed dashboard stimuli for a short, fixed exposure window and then completed retention quizzes. The experiments manipulated:

- **Hierarchy:** base, improved, importance-based, no hierarchy, room-based, or floorplan-based organization.
- **Chartjunk:** low, medium, high, base, or reduced decorative styling.
- **Domain:** IT operations and smart home dashboards.

The dependent variable was knowledge retention: correct answers about dashboard values, relationships, device states, and priorities after viewing the display.

### Statistical Validation

The dissertation analyses were later checked with methods appropriate for journal submission:

- Robust ANOVA and nonparametric checks for bounded quiz scores.
- Bootstrap confidence intervals for effect sizes.
- Planned contrasts for theory-relevant hierarchy comparisons.
- Equivalence testing to distinguish negligible chartjunk effects from unresolved null results.
- Sensitivity power analysis for the observed hierarchy effects.

These checks supported the main interpretation: hierarchy alignment mattered, and chartjunk effects were small enough that they should not dominate dashboard design decisions for retention outcomes.

## Practical Guidance

The dissertation produced four applied design recommendations:

1. Organize dashboard space around the user's decision task, not simply around the data's natural structure.
2. Use physical or spatial layouts only when users need spatial reasoning.
3. Prefer a neutral layout over a mismatched hierarchy when one display must serve incompatible tasks.
4. Treat chartjunk removal as an accessibility, clarity, or brand question first; do not assume it will improve memory by itself.

## Artifacts

<div class="image-gallery">
<div>
<img src="{{ '/assets/images/portfolio/dissertation/chartjunk-results.png' | relative_url }}" alt="Dashboard retention results by hierarchy and chartjunk condition">
<div class="caption">Retention results comparing hierarchy and chartjunk manipulations.</div>
</div>
<div>
<img src="{{ '/assets/images/portfolio/dissertation/image21.png' | relative_url }}" alt="Dashboard stimulus examples from the dissertation">
<div class="caption">Example dashboard stimulus material from the experimental studies.</div>
</div>
</div>

---

*Full dissertation materials, analysis scripts, and manuscript artifacts are available in private academic records and selected public-safe summaries.*
