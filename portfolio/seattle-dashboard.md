---
layout: case-study
title: Seattle Mayoral Accountability Dashboard
description: Civic technology for transparent government tracking
meta:
  role: Designer & Developer
  duration: 2024
  company: Personal Project
  tools: R Shiny, Plotly, bslib
---

# Seattle Mayoral Accountability Dashboard

## Problem

Seattle Mayor Katie Wilson made specific, measurable commitments about addressing homelessness — including "4,000 new emergency housing and shelter units in four years." But tracking progress against these commitments requires navigating multiple data sources across different agencies with varying update schedules.

Citizens shouldn't need a research degree to hold their elected officials accountable.

## Solution

A public-facing dashboard that aggregates data from multiple sources and presents it in a clear, confrontational-through-transparency format. No editorializing — just the numbers.

## What It Tracks

### Primary Indices

| Metric | Description | Data Source |
|--------|-------------|-------------|
| **Unsheltered Population** | People sleeping outside in Seattle | HUD PIT counts, KCRHA quarterly estimates |
| **Emergency Housing Progress** | Progress toward 4,000 unit commitment | City budget documents, KCRHA reports |
| **Homeless Overdose Deaths** | Monthly fatalities (67% of homeless deaths) | King County Medical Examiner |
| **Cost Per Person Housed** | Spending efficiency metric | Seattle Budget Office, KCRHA |

## Design Philosophy

- **Data speaks for itself** — Minimal editorializing, maximum clarity
- **Confrontational through transparency** — Not rhetoric
- **Mobile-friendly** — Designed for quick checks on phones
- **Sober, professional tone** — This is a tool, not a campaign site

## Technical Implementation

Built with **R Shiny** using:
- `bslib` for modern Bootstrap 5 theming
- `plotly` for interactive charts
- Manual data curation (no live APIs available for most sources)

### Update Schedule

- **Monthly:** Overdose deaths (with 2-3 month lag)
- **Quarterly:** Housing units, placements, KCRHA estimates
- **Annually:** Spending data, official PIT counts

## Outcome

The dashboard provides a single source of truth for tracking mayoral accountability on homelessness, aggregating data that would otherwise require hours of research across multiple government websites.

---

[View on GitHub](https://github.com/Terwox/SeattleMayoralTracking)
