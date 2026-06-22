# Resume & Portfolio Refresh Plan

## Overview
Redesign terwox.github.io with a modern tech aesthetic, purple/lavender accent colors, system fonts, and a hybrid layout (resume page + portfolio with expandable case studies). Add PDF generation capability.

---

## Design Specifications

| Aspect | Decision |
|--------|----------|
| Vibe | Modern tech / data-forward hybrid |
| Colors | Neutral base (dark grays, white) + purple/lavender bold accent |
| Layout | Hybrid: resume page + portfolio with case study sub-pages |
| Typography | System fonts (fast, reliable) |
| PDF | Markdown-to-PDF generation |

---

## Phase 1: Site Infrastructure

### 1.1 Update Jekyll config and theme setup
- [ ] Remove or override Cayman theme defaults
- [ ] Create custom CSS with purple/lavender color scheme
- [ ] Set up system font stack
- [ ] Configure responsive breakpoints

### 1.2 Create new layout templates
- [ ] `_layouts/default.html` - base template with nav, footer
- [ ] `_layouts/resume.html` - single-page resume layout
- [ ] `_layouts/portfolio.html` - portfolio index with project cards
- [ ] `_layouts/case-study.html` - individual project detail pages

### 1.3 Navigation structure
- [ ] Resume (home)
- [ ] Portfolio (grid of project cards → case study pages)
- [ ] GitHub link
- [ ] PDF download link

---

## Phase 2: Resume Content

### 2.1 Update resume content in README.md
- [ ] Verify current role/title accuracy ("Mixed Methods Researcher" confirmed OK)
- [ ] Add any recent projects/accomplishments if desired (TODO: your call)
- [ ] Clean up formatting for new design

### 2.2 PDF generation
- [ ] Set up markdown-to-PDF pipeline (options: pandoc, weasyprint, or browser print CSS)
- [ ] Create print-friendly CSS for clean PDF output
- [ ] Add PDF download link to site

### 2.3 Cleanup
- [ ] Delete `README-resume.md` (outdated Express Scripts version)

---

## Phase 3: Portfolio Content

### 3.1 Create portfolio index page
- [ ] Grid/card layout showing all projects
- [ ] Each card: title, thumbnail, brief tagline, link to case study

### 3.2 Case Study: Dissertation (Dashboard Knowledge Retention)
- [ ] Extract key content from dissertation materials
- [ ] Structure: Problem → Method → Findings → Impact
- [ ] Add relevant visualizations

### 3.3 Case Study: Seattle Mayoral Dashboard
- [ ] Pull content from `d:/git/SeattleMayoralTracking/README.md`
- [ ] Screenshots of the Shiny dashboard
- [ ] Structure: Problem → Approach → Features → Link to live app

### 3.4 Case Study: Persona Work (Cigna)
- [ ] Extract content from `d:/Dropbox/Clutter/Job apps, current/persona safe.pptx`
- [ ] Export relevant images/slides as PNGs
- [ ] Structure: Context → Method → Deliverable → Impact

### 3.5 Case Study: Microsoft Employee Experience
- [ ] Extract content from `James Myers Portfolio for Microsoft Cloud Services 7-2-18.pptx`
- [ ] Export visualizations: pain point bubbles, word clouds, sentiment charts
- [ ] Projects to include:
  - Employee pain point visualizations
  - MS Culture sentiment analysis / word clouds
  - Flow psychophysiology research
  - Kegerator UX (fun one to end on)

### 3.6 Asset management
- [ ] Export images from PowerPoints at appropriate resolution
- [ ] Organize in `/assets/images/portfolio/`
- [ ] Remove old placeholder images if replaced

---

## Phase 4: Polish & Deploy

### 4.1 Visual polish
- [ ] Test responsive design (mobile, tablet, desktop)
- [ ] Check color contrast / accessibility
- [ ] Ensure consistent spacing and typography

### 4.2 Final review
- [ ] Proofread all content
- [ ] Test all links
- [ ] Verify PDF generation works

### 4.3 Deploy
- [ ] Commit and push to GitHub
- [ ] Verify GitHub Pages builds successfully
- [ ] Test live site

---

## File Structure (Proposed)

```
terwox.github.io/
├── _config.yml
├── _layouts/
│   ├── default.html
│   ├── resume.html
│   ├── portfolio.html
│   └── case-study.html
├── assets/
│   ├── css/
│   │   └── style.css          # Custom styles
│   └── images/
│       └── portfolio/
│           ├── dissertation/
│           ├── seattle-dashboard/
│           ├── persona/
│           └── microsoft/
├── index.md                    # Resume (home)
├── portfolio.md                # Portfolio index
├── portfolio/
│   ├── dissertation.md
│   ├── seattle-dashboard.md
│   ├── persona.md
│   └── microsoft.md
└── resume.pdf                  # Generated PDF
```

---

## Source Materials

| Project | Source Location |
|---------|-----------------|
| Dissertation | `d:/git/JamesDiss/`, `d:/git/DissertationCheck/` |
| Seattle Dashboard | `d:/git/SeattleMayoralTracking/` |
| Persona Work | `d:/Dropbox/Clutter/Job apps, current/persona safe.pptx` |
| Microsoft Portfolio | `d:/Dropbox/Clutter/Job apps, current/No longer current/James Myers Portfolio for Microsoft Cloud Services 7-2-18.pptx` |
| Current Resume | `d:/git/terwox.github.io/README.md` |

---

## Open TODOs (User Input Needed)

- [ ] Any recent Cigna accomplishments to add to resume?
- [ ] Facebook interview portfolio — still looking for it, or skip?
- [ ] Dissertation: what level of detail to include (in-progress vs. completed)?

---

## Estimated Scope

- **Phase 1 (Infrastructure):** New CSS, layouts, nav
- **Phase 2 (Resume):** Content updates, PDF setup, cleanup
- **Phase 3 (Portfolio):** 4 case studies with extracted content/images
- **Phase 4 (Polish):** Testing, accessibility, deploy

Ready to execute on approval.
