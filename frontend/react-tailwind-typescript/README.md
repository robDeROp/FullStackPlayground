# React + Tailwind + TypeScript + ESLint

Deze map is bedoeld voor React-experimenten met een moderne toolchain. Net als de Vue-setup gebruiken we Vite om projecten snel te bootstrappen.

## Vereisten

- Node.js 18+
- pnpm (aanbevolen) of npm/yarn

## Installatie

1. **Project scaffolden**
   ```bash
   pnpm create vite react-tailwind-typescript -- --template react-ts
   ```

2. **Ga naar de map**
   ```bash
   cd frontend/react-tailwind-typescript
   ```

3. **Afhankelijkheden installeren**
   ```bash
   pnpm install
   ```

4. **Tailwind CSS configureren**
   ```bash
   pnpm install -D tailwindcss postcss autoprefixer
   pnpm tailwindcss init -p
   ```
   Werk `tailwind.config.cjs` bij zodat `./index.html` en `./src/**/*.{ts,tsx}` gescand worden. Importeer Tailwind in `src/index.css`.

5. **ESLint uitbreiden**
   Voeg eventuele regels toe in `.eslintrc.cjs` om consistent te blijven met Vue-configuratie. Overweeg `eslint-config-prettier` en `eslint-plugin-react-hooks`.

6. **Shared componenten gebruiken**
   Voeg in `tsconfig.json` een path alias toe:
   ```json
   {
     "compilerOptions": {
       "paths": {
         "@shared/*": ["../shared/*"]
       }
     }
   }
   ```
   Combineer dit met een Vite alias in `vite.config.ts` zodat imports uit `frontend/shared/` werken.

## Scripts

- `pnpm dev` — Start de Vite development server.
- `pnpm build` — Buildt de productievariant.
- `pnpm lint` — Voert ESLint uit.
- `pnpm test` — Voeg Vitest of Jest toe om componenten te testen.

## Extra ideeën

- Integreer React Router voor SPA-navigatie.
- Voeg React Query of Zustand toe voor state management.
- Gebruik Storybook om componenten te documenteren en vergelijken met Vue.
