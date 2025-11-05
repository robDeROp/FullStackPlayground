# Frontend Playground

Deze map bevat alle frontend-experimenten binnen de FullStackPlayground. Projecten worden georganiseerd per framework en delen gemeenschappelijke resources via de `shared/` map. Start hier wanneer je een nieuw UI-framework wil vergelijken of uitbreiden.

## Structuur

- `shared/` — Herbruikbare components, utilities en styling die framework-onafhankelijk zijn.
- `vue-tailwind-typescript/` — Vue 3 setup met TypeScript, Tailwind CSS, ESLint, Vue Router en een Three.js demo component.
- `react-tailwind-typescript/` — React setup met TypeScript, Tailwind CSS en ESLint.

## Richtlijnen

1. Houd configuraties consistent zodat je frameworks makkelijk kan vergelijken.
2. Documenteer elke framework-specifieke beslissing in de bijhorende `README.md`.
3. Plaats generieke UI-elementen eerst in `shared/` en importeer ze in je projecten via symlinks of package-aliassen.

Veel experimenteerplezier!
