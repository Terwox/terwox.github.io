---
layout: case-study
title: Healthcare Persona Development
description: Mixed methods persona research combining LPA with qualitative validation
meta:
  role: Lead Researcher
  duration: 2021
  company: Cigna
  tools: R, Latent Profile Analysis, Qualtrics, In-depth Interviews
---

# Healthcare Persona Development

## The Problem

Healthcare organizations typically segment members by demographics — age, income, geography, condition. But demographics don't predict behavior. A 65-year-old with diabetes and a 35-year-old with diabetes may have more in common behaviorally than two 65-year-olds with different attitudes toward self-management.

The existing personas were based on stakeholder assumptions, not data. Product teams were making decisions based on archetypes that didn't reflect actual member diversity.

## Why Latent Profile Analysis

Traditional persona methods have a fundamental flaw: researchers decide the segments upfront, then find data to support them. This embeds assumptions into the output.

**Latent Profile Analysis (LPA)** inverts this:

| Traditional Approach | LPA Approach |
|---------------------|--------------|
| Define segments first, then validate | Let data reveal natural groupings |
| Researcher decides number of personas | Statistical fit indices determine optimal count |
| Risk of confirmation bias | Clusters emerge from response patterns |
| Segments reflect assumptions | Segments reflect actual behavioral variation |

LPA was the right choice because we needed personas that would survive contact with reality — segments grounded in measurable behavioral differences, not marketing intuitions.

## Approach

### Phase 1: Quantitative Segmentation

**Large-scale survey** measuring behavioral and attitudinal dimensions:

- Health self-efficacy and locus of control
- Medication adherence patterns and barriers
- Communication channel preferences
- Trust in healthcare providers and systems
- Life circumstances affecting healthcare engagement

**Analysis:**

- Exploratory LPA to test 2-6 profile solutions
- Model selection based on BIC, entropy, and interpretability
- Final model validated through bootstrap resampling

### Phase 2: Qualitative Validation

**In-depth interviews** with members classified into each profile to:

- Confirm that statistical segments mapped to lived experience
- Understand the causal mechanisms behind behavioral patterns
- Surface pain points and unmet needs invisible in survey data
- Gather narrative detail that brings personas to life

This phase was essential because LPA tells you *that* groups differ — interviews tell you *why*.

### Phase 3: Persona Synthesis

Each persona was built on:

- **Quantitative foundation:** Behavioral indicators with measurable differences between segments
- **Qualitative depth:** Motivations, mental models, and journey context
- **Design implications:** Specific recommendations for product and content teams

## Key Finding

**Attitude toward self-management** emerged as the primary differentiator — more predictive than demographics, condition type, or tenure with the pharmacy.

Members who saw themselves as active participants in their healthcare had fundamentally different needs:

- Wanted detailed information and self-service tools
- Frustrated by paternalistic communication
- Valued transparency about costs and alternatives

Members who preferred to defer to providers:

- Wanted guidance and reassurance
- Overwhelmed by too many options
- Valued relationship with care team over self-service efficiency

This insight shifted the product strategy from "one experience optimized for efficiency" to "adaptive experiences that meet members where they are."

## Deliverables

- Persona documentation with behavioral data backing each characteristic
- Segment sizing and distribution across the member population
- Journey maps for each persona through key healthcare touchpoints
- Design recommendations for persona-specific communication strategies
- Segment classifier for applying personas to new members

## Impact

The personas became a shared language across teams:

- **Product:** Persona-specific feature prioritization
- **Design:** Adaptive UX patterns based on member type
- **Content:** Tailored communication tone and information density
- **Operations:** Service design for different engagement preferences

---

*Sample sizes and specific metrics sanitized for confidentiality.*
