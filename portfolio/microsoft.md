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

Research and data visualization work focused on turning large-scale employee survey data into actionable insights for leadership. The challenge: thousands of open-ended responses and Likert-scale ratings needed to become clear priorities that facilities, HR, and leadership could act on.

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

### Outcome

The visualization made priorities undeniable: **workspace distractions** dominated — high frequency, high severity, high response count. This gave facilities leadership a clear mandate and data-backed justification for workplace redesign investments.

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

## Methods Reflection

This work demonstrated the power of **visualization as a research deliverable**. The same data in a table would have been ignored; presented visually with clear priority axes, it drove facilities planning decisions.

Key approach: Always design visualizations that make the recommended action obvious. If stakeholders have to interpret, they'll interpret wrong.

---

*Work performed as a Microsoft employee. Visualizations shown are representative of the approach; specific data has been generalized.*
