# Shared Components

Gebruik deze map om framework-onafhankelijke UI-componenten te bewaren. Denk aan generieke knoppen, layout-elementen, design tokens of utilities die je wil hergebruiken in zowel Vue- als React-projecten.

## Werkwijze

1. Bouw componenten in TypeScript en exporteer ze als framework-neutrale functies of Web Components.
2. Publiceer ze optioneel via een lokaal npm-package (bijv. via `pnpm workspaces`) zodat je ze kan importeren in elke frontend-map.
3. Documenteer afhankelijkheden en eventuele adapter-lagen voor specifieke frameworks.

> Tip: voeg Storybook of Ladle toe in deze map om componenten onafhankelijk te ontwikkelen en testen.
