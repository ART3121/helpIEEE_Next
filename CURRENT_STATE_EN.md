# Current state - HELPIEEE Next

Last update: `2026-04-09`

## Quick summary

The `helpieee-next` project is already published as a separate repository and works as a faithful migration of the original demo into Next.js.

## What is ready

- home at `/` and `/index.html`
- legacy pages at `/pages/*.html`
- flow at `/pages/fluxo.html`
- `/fluxo.html` alias
- legacy HTML renderer inside Next
- preserved light/dark theme
- Electrical Engineering curricula
- Computational Engineering curriculum
- Computer Science full-time and evening curricula
- fixed synchronized horizontal scrollbar in the flow

## Core files for resuming work

- [`README_EN.md`](./README_EN.md)
- [`components/LegacyPageRenderer.jsx`](./components/LegacyPageRenderer.jsx)
- [`lib/legacyDocuments.js`](./lib/legacyDocuments.js)
- [`legacy-source/pages/fluxo.html`](./legacy-source/pages/fluxo.html)
- [`public/assets/js/pages/fluxo-data.js`](./public/assets/js/pages/fluxo-data.js)
- [`public/assets/js/pages/fluxo.js`](./public/assets/js/pages/fluxo.js)
- [`public/assets/css/pages/fluxo.css`](./public/assets/css/pages/fluxo.css)

## Latest validation

- `npm run lint`
- `npm run build`

## Attention points

- the codebase is still mostly legacy, only wrapped by Next
- workload-based prerequisites are not yet structurally modeled in the flow
- changes in `legacy-source` should continue to respect the `mtime`-aware loader
