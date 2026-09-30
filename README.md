# CITRA

**AI Search Intelligence** — a dark, product-style dashboard for understanding how answer engines may represent, cite, and recommend a brand.

> **Demo note:** CITRA currently uses modeled/demo data. The interface does not claim to query ChatGPT, Gemini, Perplexity, Google AI, or Copilot live unless a real integration is added.

## What CITRA covers

- **Overview** — AI visibility score, engine-level presence, mention rate, recommendation rate, citation rate, competitor share, and source diversity.
- **Query Intelligence** — buyer questions, simulated mentions, recommendations, citations, opportunity scores, and competing brands.
- **Competitor Intelligence** — visibility, mention frequency, citation strength, topical authority, and entity completeness.
- **Citation Explorer** — source authority, citation frequency, owned documentation, research, community, marketplace, and competitor sources.
- **Entity Health** — organization, product, service, author, location, FAQ, and review coverage.
- **AI Action Plan** — prioritized visibility actions with impact and severity.
- **Analysis flow** — a guided crawl → entity discovery → topical analysis → query simulation → competitor analysis → visibility model experience.

## Demo

The repository includes a self-contained `index.html` demo so the experience can be opened directly from GitHub Pages or any static host. No API key is required for the demo.

### Run locally

```bash
# Option 1: open index.html directly
# Option 2: serve the repository with any static server
npx serve .
```

## Repository structure

```text
CITRA/
├── index.html        # Standalone interactive demo
├── README.md         # Project documentation
├── screenshots/      # Product screenshots when binary upload is available
└── source/           # Reserved for the full React source implementation
```

## Product experience

### 1. Overview

The overview presents the modeled AI visibility score and a five-engine presence view, followed by core visibility metrics and high-priority opportunities.

### 2. Query intelligence

Queries are displayed as buyer-intent rows with mention, recommendation, citation, opportunity, and competitor signals.

### 3. Competitor intelligence

CITRA compares brands across five signals to make the modeled competitive surface easy to inspect.

### 4. Citation explorer

Sources are grouped by type and represented with authority and citation-frequency signals.

### 5. Entity health

The entity screen highlights which business entities are healthy, partial, or missing and shows their modeled coverage.

### 6. Action plan

The action plan translates visibility gaps into concrete actions, including comparison content, FAQ/author entities, topical ownership, machine-readable pricing, and community proof.

## Design system

- Near-black product UI
- Purple → cyan gradients
- Lime positive states
- Orange warning states
- Red critical states
- Space Grotesk / Inter / JetBrains Mono inspired typography
- Responsive desktop and mobile layouts
- Border-first cards and compact data visualizations

## Tech stack

The original project was authored as a React + TypeScript + Vite + TanStack Router application. This repository also contains a standalone HTML demo so the product experience can be reviewed without installing the full application stack.

## Roadmap

- Connect live answer-engine/provider APIs
- Persist analysis runs
- Crawl real websites
- Add authenticated workspaces
- Store historical visibility runs
- Add real citation extraction and source verification
- Add exportable reports

## Screenshots

The supplied product screens cover the homepage, analysis flow, overview, queries, competitors, citations, entity health, and action plan. The screenshot set can be added under `screenshots/` when binary asset write support is enabled for the connected GitHub integration.

## License

No open-source license has been declared yet. Add a license before distributing CITRA as an open-source project.
