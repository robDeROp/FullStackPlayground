# Databases

Alle databaseconfiguraties voor de playground leven hier. Start met MySQL via Docker en breid later uit met andere engines (PostgreSQL, MongoDB, Redis, ...).

## Richtlijnen

- Gebruik Docker Compose voor consistentie tussen projecten.
- Voorzie per database een `.env.example`.
- Documenteer migrations en seed scripts.

## Beschikbare setups

- `mysql/` — Lokaal MySQL-instance met persistente opslag en init scripts.
