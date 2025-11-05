# NestJS API

Deze map is gereserveerd voor NestJS-projecten. NestJS biedt een gestructureerd framework voor schaalbare server-side applicaties met TypeScript.

## Vereisten

- Node.js 18+
- pnpm (of npm/yarn)
- Nest CLI (`pnpm add -g @nestjs/cli`)

## Installatie

1. **Project genereren**
   ```bash
   nest new nestjs-playground
   ```
   Kies `pnpm` als package manager en verplaats de gegenereerde bestanden naar `apis/nestjs`.

2. **Projectstructuur**
   ```
   src/
     app.module.ts
     main.ts
     modules/
       example/
         example.module.ts
         example.controller.ts
         example.service.ts
   ```
   Gebruik de `modules/` map om feature-modules te groeperen.

3. **Linting & Formatter**
   Nest genereert standaard ESLint-configuratie. Pas deze aan indien nodig om consistent te blijven met andere projecten.

4. **MySQL koppeling**
   - Installeer TypeORM of Prisma.
   - Voeg een `DatabaseModule` toe in `src/modules/database`.
   - Sla database-credentials op in `.env` en maak een `.env.example`.

5. **Docker ondersteuning**
   Maak een `Dockerfile` en `docker-compose.yml` indien je de service gecontaineriseerd wil testen. Verwijs naar de MySQL-container in `databases/mysql`.

## Scripts

- `pnpm start:dev` — Development server met hot reload.
- `pnpm start` — Productiemodus.
- `pnpm test` — Unit tests via Jest.
- `pnpm test:e2e` — End-to-end tests.
- `pnpm lint` — ESLint.

## Tips

- Gebruik Swagger (`@nestjs/swagger`) om API-documentatie te genereren.
- Integreer class-validator + class-transformer voor DTO-validatie.
- Deel interfaces of DTO's via `/packages` indien meerdere API's ze nodig hebben.
