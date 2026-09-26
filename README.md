# Tejas Arya — portfolio

A responsive, local-first portfolio built with HTML and CSS only. No JavaScript, dependencies, backend, or build step.

## Open it

Open `index.html` directly, or serve this directory:

```sh
python3 -m http.server 8087 --bind 127.0.0.1
```

Then visit `http://localhost:8087`.

## Pages and styles

- `index.html`: concise introduction, clearly attributed impact metrics, four filterable projects, experience, research, education, toolkit, and contact.
- `inventory-expert.html`: a guided vehicle-domain case study with four chapters: architecture, request flow, search logic, and engineering.
- `styles.css`: shared design system, light/dark themes, portfolio, architecture map, responsive layouts, and print styles.
- `diagrams.css`: animated six-stage request journey, changing input/output payloads, parallel retrieval, and contextual follow-ups.
- `search.css`: structured, semantic, and mixed-search examples.
- `TejasArya8261 (2).pdf`: downloadable source résumé.

## Design

The redesign replaces the dense, repeated technical sections with a portfolio overview and a dedicated case study. It uses a white/cool-gray surface, navy text, blue accents, larger type, consistent spacing, and progressive disclosure. The case study has sticky chapter navigation; on small screens this becomes a compact navigation bar. The six-stage request diagram becomes a vertical sequence on phones.

## Interactions

- Native radio inputs filter projects and switch between search examples. Use Tab to reach the group, then arrow keys to change the selection.
- Only the vehicle branch expands in the architecture diagram. A nested disclosure shows the five inventory tools. Other agent cards are static context.
- Native disclosures reveal project details, job experience, engineering decisions, and the request transcript.
- The request animation loops over six stages in 36 seconds. Each active node corresponds to the input/output panel below. Pause motion freezes all three diagrams, including the parallel search and follow-up examples.
- Reduced-motion preferences show all six payloads without animation; print styles also expose the complete sequence.
- A checkbox toggles the light/dark theme for the current page. This preference does not persist between pages because there is no JavaScript or storage.
- Keyboard focus indicators, a skip link, semantic headings, labels, and text explanations accompany the visual diagrams.

## Content accuracy

Tejas’s contribution is described as the **vehicle domain**, not ownership of the entire sales-agent platform. Other specialists explain the surrounding architecture.

Search distinguishes normalized structured fields, known equipment fields, and embeddings for descriptive features/options. Semantic results are candidates, not proof of exact equipment. Availability errors and broadened searches require appropriate explanation. Example vehicles and animation timing are illustrative, not live results or measured latency.

The production metrics belong to call intent classification and CRM Pro; they are not inventory-search benchmarks. No source credentials or dealership/customer records are included.

## Compatibility and verification

Use a current browser with CSS `:has()` support. Local checks validate HTML, CSS, IDs, labels, relative links, radio-panel selectors, and animation stage alignment. Browser review covers the main layouts, vehicle/tool expansion, search choices, project filtering, pause/resume, and dark mode. Responsive overflow is checked at narrow, tablet, and desktop widths.
