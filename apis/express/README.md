# Express.js API (TypeScript)

Gebruik deze map om Express.js services te bouwen en te testen. De setup richt zich op TypeScript, ESLint en hot-reloading via ts-node-dev of Nodemon.

## Vereisten

- Node.js 18+
- pnpm (of npm/yarn)

## Installatie

1. **Project initialiseren**
   ```bash
   pnpm init
   pnpm install express cors dotenv
   pnpm install -D typescript ts-node-dev @types/node @types/express eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin
   ```

2. **TypeScript configureren**
   ```bash
   pnpm tsc --init --rootDir src --outDir dist --esModuleInterop --resolveJsonModule --moduleResolution node --strict
   ```

3. **Scripts toevoegen** (`package.json`)
   ```json
   {
     "scripts": {
       "dev": "ts-node-dev --respawn --transpile-only src/main.ts",
       "build": "tsc",
       "start": "node dist/main.js",
       "lint": "eslint \"src/**/*.{ts,tsx}\""
     }
   }
   ```

4. **Folderstructuur**
   ```
   src/
     main.ts
     app.ts
     routes/
     controllers/
     services/
     config/
   ```
   - `config/` bevat verbindingen naar MySQL of andere services.
   - Bewaar herbruikbare middleware in `src/middleware/`.

5. **MySQL koppelen**
   Installeer een ORM/Query builder (bijv. Prisma of Knex). Configureer `.env` met de MySQL-URL uit `databases/mysql`.

## Starten

```bash
pnpm dev
```

## Testing

- Voeg Jest of Vitest toe voor unit tests.
- Gebruik Supertest voor endpoint-tests.
