# Estado atual - HELPIEEE Next

Ultima atualizacao: `2026-04-09`

## Resumo rapido

O projeto `helpieee-next` ja esta publicado como repositorio separado e funciona como migracao fiel da demo original para Next.js.

## O que esta pronto

- home em `/` e `/index.html`
- paginas legadas em `/pages/*.html`
- fluxo em `/pages/fluxo.html`
- alias `/fluxo.html`
- renderer de HTML legado em Next
- tema claro/escuro preservado
- curriculos de Engenharia Eletrica
- curriculo de Engenharia Computacional
- curriculos de Ciencia da Computacao integral e noturno
- barra horizontal fixa e sincronizada no fluxo

## Arquivos centrais para retomada

- [`README.md`](./README.md)
- [`components/LegacyPageRenderer.jsx`](./components/LegacyPageRenderer.jsx)
- [`lib/legacyDocuments.js`](./lib/legacyDocuments.js)
- [`legacy-source/pages/fluxo.html`](./legacy-source/pages/fluxo.html)
- [`public/assets/js/pages/fluxo-data.js`](./public/assets/js/pages/fluxo-data.js)
- [`public/assets/js/pages/fluxo.js`](./public/assets/js/pages/fluxo.js)
- [`public/assets/css/pages/fluxo.css`](./public/assets/css/pages/fluxo.css)

## Validacao mais recente

- `npm run lint`
- `npm run build`

## Pontos de atencao

- a base ainda e majoritariamente legada, so encapsulada em Next
- pre-requisitos por carga horaria ainda nao sao modelados estruturalmente no fluxo
- alteracoes em `legacy-source` devem continuar respeitando o loader com cache por `mtime`
