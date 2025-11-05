# Vue 3 + Tailwind + TypeScript + ESLint + Router + Three.js

Deze map bevat de Vue-playgroundconfiguratie. Gebruik dit project om Vue 3 te testen met een moderne tooling-stack. De setup is gebaseerd op Vite zodat je snel kan itereren.

## Vereisten

- Node.js 18+
- pnpm (aanbevolen) of npm/yarn

## Installatie

1. **Project scaffolden**
   ```bash
   pnpm create vue@latest
   ```
   Kies volgende opties:
   - Projectnaam: `vue-tailwind-typescript`
   - TypeScript: **Ja**
   - JSX Support: optioneel
   - Vue Router: **Ja**
   - Pinia: optioneel
   - Vitest: optioneel
   - ESLint + Prettier: **Ja**

2. **Ga naar de map**
   ```bash
   cd frontend/vue-tailwind-typescript
   ```

3. **Tailwind CSS toevoegen**
   ```bash
   pnpm install -D tailwindcss postcss autoprefixer
   pnpm tailwindcss init -p
   ```
   Werk daarna `tailwind.config.cjs` bij zodat `./index.html` en `./src/**/*.{vue,ts,tsx}` gescand worden. Importeer Tailwind in `src/assets/main.css`:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

4. **Three.js component opzetten**
   - Installeer Three.js: `pnpm add three`
   - Maak een component `src/components/ThreeCanvas.vue` met een eenvoudige scene.
   - Gebruik `onMounted` om de renderer te initialiseren en voeg een resize-listener toe.

5. **Shared components gebruiken**
   Voeg in `vite.config.ts` een alias toe:
   ```ts
   resolve: {
     alias: {
       '@shared': fileURLToPath(new URL('../../shared', import.meta.url))
     }
   }
   ```
   Hiermee importeer je generieke UI-elementen uit `frontend/shared/`.

## Scripts

- `pnpm dev` — Start de Vite development server.
- `pnpm build` — Buildt de productievariant.
- `pnpm lint` — Voert ESLint uit.
- `pnpm test` — (optioneel) Vitest.

## Aanbevelingen

- Voeg Cypress of Playwright toe voor end-to-end tests.
- Documenteer belangrijke keuzes in deze map zodat toekomstige jij snel kan herstarten.
