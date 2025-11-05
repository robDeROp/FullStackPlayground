# API Playground

Deze map bundelt backend-experimenten. Elke submap bevat een zelfstandig project of proof-of-concept. Deel businesslogica via gedeelde packages (zie `/packages`).

## Beschikbare projecten

- `express/` — Minimalistische Express API met TypeScript.
- `nestjs/` — NestJS applicatie met gestructureerde modules en Docker-ondersteuning.

## Richtlijnen

1. Gebruik een consistente code style (TypeScript + ESLint + Prettier).
2. Deel utilities (bijv. DTO's, valideringsschemas) via packages in de root.
3. Houd environment configuraties bij in `.env.example` bestanden.

## Databasekoppeling

Beide projecten kunnen dezelfde MySQL-container gebruiken uit `databases/mysql`. Documenteer migrations en seed scripts in de projectmap.
