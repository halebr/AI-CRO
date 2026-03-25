You have now produced the complete analysis for this business — strategy memos, CRO playbooks, GTM experiments, key debates, narrative summary, and critical updates. Now build a website to house it all as a living, navigable "second brain."

## Your Mission

Create a Next.js website and deploy it to Vercel. This site serves as the single destination where anyone — a board member, an investor, an executive, a new hire — can explore the full strategic picture of this business.

## Site Structure

### Hero Section
- Company name and one-line descriptor (e.g., "[Company]: A $XM [Description]")
- 2-3 sentences of context on what the company does and its current trajectory
- CTA buttons linking to the podcast and analysis sections

### Key Metrics Grid
- 6 stat cards showing the most important numbers at a glance
- Pull these directly from the analysis: revenue run rate, growth rate, channel mix, take rate, projects completed, operational efficiency ratio
- Use large numbers with short labels

### Podcast Section
- Embedded audio player for the NotebookLM-generated podcast
- Brief description of what the podcast covers

### Presentation Section
- Embedded PDF viewer for the NotebookLM-generated presentation
- Download link

### Analysis Hub
Organize all analysis documents into four card-based subsections:

1. **Strategy Memos** — Each memo gets a card with title, one-line summary, and link to the full document
2. **CRO Playbooks** — Same format, organized by GTM function
3. **GTM Experiments** — Each experiment gets a card with title, priority badge (NOW / Q2 / Q3 / Q4), and projected impact
4. **Critical Updates** — Time-sensitive documents that represent inflection points or revised assessments

### Executive Summary
- A synthesis section at the bottom that ties everything together
- Cover: business model, growth trajectory, key constraints, and top opportunities
- This should read like a one-page board memo

## Design Requirements

- Clean, minimal aesthetic — white cards on light background
- Blue accent color for interactive elements and CTAs
- Responsive grid layouts that work on desktop and mobile
- Status badges on experiment cards using color-coded tags (red = NOW, blue = Q2, gray = Q3+)
- Strong typographic hierarchy — someone scanning should grasp the structure in 5 seconds
- No unnecessary animation or decoration

## Technical Requirements

- Next.js with App Router
- All analysis content stored as markdown files in a /content directory, rendered with a markdown parser (gray-matter + remark or similar)
- Static generation where possible (these documents don't change frequently)
- Deploy to Vercel via CLI (`vercel --prod`)
- Each analysis document should have its own route (e.g., /analysis/strategy-memo-2)
- Responsive images and embedded media

## Content to Include

Convert all of the following documents into the site's content directory:
- All Strategy Memos
- All CRO Playbooks
- The GTM Experiments document (split into individual cards on the hub, full document on its own page)
- Key Debates
- The Narrative Summary ("The [Company] Story")
- Any Critical Updates or revised assessments
- The NotebookLM podcast audio file
- The NotebookLM presentation PDF

## Important

This is a living site. Structure the content directory and components so that adding a new memo, playbook, or experiment is as simple as dropping a new markdown file into the right folder — no code changes required.
