---
layout: case-study
title: Microsoft Employee Experience Research
description: Data visualization and analysis for enterprise insights
meta:
  role: UX Researcher
  duration: 2018-2019
  company: Microsoft
  tools: R, Kusto, Power BI, Qualtrics
---

# Microsoft Employee Experience Research

A collection of data visualization and analysis work from my time at Microsoft, focused on understanding and communicating employee experience insights.

---

## Employee Pain Point Visualization

### Problem

Employee experience surveys generate massive amounts of data, but stakeholders struggled to identify priorities. What issues should leadership focus on first?

### Solution

Created a bubble chart visualization showing:
- **X-axis:** Frequency of issue occurrence
- **Y-axis:** Severity of impact on satisfaction
- **Bubble size:** Number of respondents reporting the issue
- **Color:** Category of pain point

<div class="image-gallery single">
<img src="{{ '/assets/images/portfolio/microsoft/image3.png' | relative_url }}" alt="Employee pain point bubble chart">
<p class="caption">Pain point visualization showing frequency vs. severity</p>
</div>

### Key Finding

The primary story: **distractions in physical workspace** dominated as the top pain point — high frequency, high severity, high response count. This provided clear direction for facilities and workplace teams.

---

## Culture Word Clouds

### Problem

Open-ended survey responses about Microsoft culture contained rich qualitative data, but executives wanted quick visual summaries.

### Solution

Created word clouds at multiple granularities:
- **Unigram clouds** — Individual word frequency
- **Bigram clouds** — Two-word phrase frequency (more contextual)

<div class="image-gallery">
<img src="{{ '/assets/images/portfolio/microsoft/image5.png' | relative_url }}" alt="Unigram word cloud">
<img src="{{ '/assets/images/portfolio/microsoft/image6.png' | relative_url }}" alt="Bigram word cloud">
</div>

---

## Sentiment Analysis

### Problem

Word frequency doesn't capture whether mentions are positive or negative. "Work-life balance" could mean "great work-life balance" or "terrible work-life balance."

### Solution

Applied sentiment analysis to categorize responses, then created sentiment-sorted visualizations showing:
- Positive vs. negative mention distribution
- Topics that generated strong emotional responses
- Areas of consensus vs. controversy

<div class="image-gallery single">
<img src="{{ '/assets/images/portfolio/microsoft/image4.png' | relative_url }}" alt="Sentiment-sorted visualization">
<p class="caption">Sentiment analysis of employee feedback</p>
</div>

---

## Physical vs. Remote Workspace Analysis

### Problem

With Microsoft's mixed workforce (office, remote, hybrid), leadership needed to understand whether workspace pain points differed by work arrangement.

### Solution

Segmented the pain point data by:
- Physical workspace issues vs. other categories
- Open plan office vs. private office employees

This revealed that open plan employees reported significantly higher distraction-related pain points, informing facilities planning decisions.

---

## Psychophysiology and Flow

### Problem

Survey data captures what people *say* about their experience, but not necessarily their actual cognitive and emotional states during work.

### Research Direction

Explored the use of psychophysiological measures (building on my dissertation research) to understand flow states and deep work in the enterprise context.

---

## Kegerator UX

A lighter project: Improving the user experience of Microsoft's office kegerators.

Sometimes UX research is serious enterprise strategy. Sometimes it's making sure people can easily get a beer after work.

---

*Work performed as a Microsoft employee. Visualizations shown are representative of the approach; specific data has been generalized.*
