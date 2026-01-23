---
layout: case-study
title: Seattle Mayoral Accountability Dashboard
description: Civic technology applying UX and data viz principles to government transparency
meta:
  role: Designer & Developer
  duration: 2024
  company: Personal Project
  tools: R Shiny, Plotly, bslib
---

# Seattle Mayoral Accountability Dashboard

## The Problem

Seattle Mayor Bruce Harrell made specific, measurable commitments about addressing homelessness — including "4,000 new emergency housing and shelter units in four years." But tracking progress against these commitments requires navigating multiple data sources across different agencies with varying update schedules.

The information exists. It's just scattered across budget PDFs, quarterly reports, and press releases that no typical citizen has time to synthesize.

**Design question:** How do you make government data accessible without editorializing it?

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

## UX Decisions

**Why no editorializing?** Civic tech often fails because it becomes advocacy. The moment you add "failing" or "succeeding" labels, you've lost credibility with half your audience. Raw numbers with clear context let viewers draw their own conclusions.

**Why mobile-first?** Accountability should be checkable in 30 seconds on a phone. If you have to sit at a desktop, you won't look.

**Why manual data curation?** Government data sources don't have APIs. Rather than waiting for perfect infrastructure, ship something useful now.

## What I Learned

Building for civic engagement is different from enterprise UX. Users are skeptical by default, attention spans are shorter, and the cost of perceived bias is immediate abandonment. The restraint to *not* tell users what to think was the hardest design constraint.

---

[View on GitHub](https://github.com/Terwox/SeattleMayoralTracking)
