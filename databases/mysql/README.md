# MySQL met Docker

Deze map bevat de configuratie om een MySQL-database lokaal te draaien via Docker. Gebruik deze container voor zowel frontend- als backendprojecten in de playground.

## Vereisten

- Docker Desktop of Docker Engine (macOS/Windows/Linux)
- Optioneel: Docker Compose

## Quickstart

1. **Maak een `.env` bestand** gebaseerd op onderstaande variabelen:
   ```env
   MYSQL_ROOT_PASSWORD=supersecret
   MYSQL_DATABASE=playground
   MYSQL_USER=playground
   MYSQL_PASSWORD=playground
   ```

2. **Start de container**
   ```bash
   docker compose up -d
   ```

3. **Controleer de status**
   ```bash
   docker compose ps
   ```

## docker-compose.yml

Plaats volgend bestand in deze map:
```yaml
services:
  mysql:
    image: mysql:8.0
    container_name: playground-mysql
    restart: unless-stopped
    ports:
      - "3306:3306"
    environment:
      MYSQL_ROOT_PASSWORD: \${MYSQL_ROOT_PASSWORD}
      MYSQL_DATABASE: \${MYSQL_DATABASE}
      MYSQL_USER: \${MYSQL_USER}
      MYSQL_PASSWORD: \${MYSQL_PASSWORD}
    volumes:
      - ./data:/var/lib/mysql
      - ./init:/docker-entrypoint-initdb.d
```

## Data & migraties

- `data/` — Persistente opslag (wordt automatisch aangemaakt).
- `init/` — Plaats `.sql` of `.sh` bestanden om tabellen en seed-data te initialiseren.

## Verbinding maken

Gebruik volgende connectiestring in je projecten:
```
mysql://playground:playground@localhost:3306/playground
```

Pas poort of credentials aan indien nodig.
