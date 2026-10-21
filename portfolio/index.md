---
layout: default
title: Portfolio
description: Selected work samples
---

# Researcher who builds

I am a mixed-methods researcher and human-factors psychologist. I study how people understand complex systems, then build the methods, analyses, and software needed to make the answer useful. My work spans human-computer interaction, healthcare, enterprise software, and civic technology.

<section class="oss-contributions" aria-labelledby="open-source-heading">

<div class="oss-section-heading">
<h2 id="open-source-heading">Open-source work</h2>
<p>When a tool I rely on fails in a way I can diagnose, I try to fix the failure upstream. These are merged contributions to projects I do not own.</p>
</div>

<div class="oss-scoreboard" aria-label="Open-source contribution totals">
<div class="oss-score">
<span class="oss-score-label">Projects contributed to</span>
<strong class="oss-score-number">{{ site.data.oss_contributions.summary.totalProjects }}</strong>
</div>
<div class="oss-score">
<span class="oss-score-label">Merged pull requests</span>
<strong class="oss-score-number">{{ site.data.oss_contributions.summary.totalPRsMerged }}</strong>
</div>
</div>

<div class="oss-project-list">
{% for contribution in site.data.oss_contributions.contributions %}
{% assign detail = site.data.oss_contribution_details | where: "repo", contribution.repo | first %}
<article class="oss-project">
<header class="oss-project-header">
<h3><a href="{{ contribution.repoURL }}">{{ detail.name | default: contribution.repoName }}</a></h3>
<span class="oss-pr-count">{{ contribution.prsMerged }} merged {% if contribution.prsMerged == 1 %}PR{% else %}PRs{% endif %}</span>
</header>
<p><strong>What it is:</strong> {{ detail.what_it_is | default: contribution.description }}</p>
{% if detail.contribution %}
<p><strong>What I changed:</strong> {{ detail.contribution }}</p>
{% endif %}
{% if detail.pull_requests %}
<ul class="oss-pr-links">
{% for pull_request in detail.pull_requests %}
<li><a href="{{ pull_request.url }}">Merged pull request #{{ pull_request.number }}</a><span aria-hidden="true"> · </span>{{ pull_request.merged }}</li>
{% endfor %}
</ul>
{% endif %}
</article>
{% endfor %}
</div>

<p class="oss-source">Counts refresh weekly from merged work on <a href="https://github.com/Terwox">GitHub profile Terwox</a>.</p>

</section>

## Selected research work

<div class="portfolio-grid">

<div class="portfolio-card">
<a href="{{ '/portfolio/dissertation/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/dissertation/chartjunk-results.png' | relative_url }}" alt="Dashboard knowledge retention research" class="card-image">
<div class="card-content">
<div class="card-title">Dashboard Knowledge Retention</div>
<div class="card-description">Doctoral human factors research showing how hierarchy alignment affects what users remember from dashboards.</div>
<div class="card-tags">
<span class="tag">Human Factors</span>
<span class="tag">Experiments</span>
<span class="tag">Dashboards</span>
</div>
</div>
</a>
</div>

<div class="portfolio-card">
<a href="{{ '/portfolio/quantitative-methods/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/quantitative-methods/contrasts.png' | relative_url }}" alt="Quantitative methods contrast results" class="card-image">
<div class="card-content">
<div class="card-title">Quantitative Methods</div>
<div class="card-description">How I use statistics to pressure-test experiments, NPS feedback, and design guidance.</div>
<div class="card-tags">
<span class="tag">R</span>
<span class="tag">Statistics</span>
<span class="tag">Validation</span>
</div>
</div>
</a>
</div>

<div class="portfolio-card">
<a href="{{ '/portfolio/research-tooling/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/research-tooling/workflow-preview.png' | relative_url }}" alt="Trustworthy reporting pipeline workflow" class="card-image">
<div class="card-content">
<div class="card-title">Research Tooling</div>
<div class="card-description">Reusable research operations systems for online experiments, reproducible reporting, and trustworthy AI-assisted synthesis.</div>
<div class="card-tags">
<span class="tag">Research Ops</span>
<span class="tag">Pipelines</span>
<span class="tag">LLM Evaluation</span>
</div>
</div>
</a>
</div>

<div class="portfolio-card">
<a href="{{ '/portfolio/persona/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/persona/image45.png' | relative_url }}" alt="Persona Research" class="card-image">
<div class="card-content">
<div class="card-title">Healthcare Persona Development</div>
<div class="card-description">Mixed methods persona research combining large-scale survey data with latent profile analysis to segment healthcare members.</div>
<div class="card-tags">
<span class="tag">Personas</span>
<span class="tag">Healthcare</span>
<span class="tag">Mixed Methods</span>
</div>
</div>
</a>
</div>

<div class="portfolio-card">
<a href="{{ '/portfolio/seattle-dashboard/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/seattle/dashboard-preview.png' | relative_url }}" alt="Seattle Mayor Dashboard" class="card-image">
<div class="card-content">
<div class="card-title">Seattle Mayoral Accountability Dashboard</div>
<div class="card-description">Public-facing R Shiny dashboard tracking Seattle Mayor's performance on homelessness commitments through transparent data visualization.</div>
<div class="card-tags">
<span class="tag">R Shiny</span>
<span class="tag">Civic Tech</span>
<span class="tag">Data Viz</span>
</div>
</div>
</a>
</div>

<div class="portfolio-card">
<a href="{{ '/portfolio/microsoft/' | relative_url }}">
<img src="{{ '/assets/images/portfolio/microsoft/image6.png' | relative_url }}" alt="Microsoft Employee Experience" class="card-image">
<div class="card-content">
<div class="card-title">Microsoft Employee Experience Research</div>
<div class="card-description">Data visualization and analysis of employee experience surveys, including pain point mapping, sentiment analysis, and culture word clouds.</div>
<div class="card-tags">
<span class="tag">Data Viz</span>
<span class="tag">R</span>
<span class="tag">Enterprise</span>
</div>
</div>
</a>
</div>

</div>
