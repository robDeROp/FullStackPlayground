# 🧩 FullStackPlayground

**FullStackPlayground** is mijn persoonlijke full-stack leeromgeving — een centrale plek waar ik experimenteer met verschillende **programmeertalen**, **frameworks** en **technologieën** om mijn vaardigheden als developer te verdiepen.

Het doel van dit project is om ervaring op te doen met uiteenlopende **frontend-** en **backend-omgevingen**, en om die kennis op een gestructureerde manier vast te leggen zodat ik ze later eenvoudig kan hergebruiken of als referentie kan raadplegen.

---

## 🎯 Doel van de repository

Deze monorepo dient als een **praktisch leerlab** waarin ik:

* Experimenteer met verschillende **web frameworks** (Next.js, Vue, SvelteKit, Express, FastAPI, enz.)
* Werk met diverse **programmeertalen** (TypeScript, JavaScript, Python, PHP, SQL)
* Oefen met **databasebeheer** via Docker (PostgreSQL of andere SQL-varianten)
* Test **API-architecturen**, design patterns en deploymentstrategieën
* Documenteer **best practices**, setups en herbruikbare snippets

Kortom: **FullStackPlayground** is mijn persoonlijke digitale werkplaats waar theorie omgezet wordt in praktijkervaring.

---

## 🧠 Waarom deze repo bestaat

In een professioneel traject als full-stack developer kom je voortdurend in aanraking met nieuwe frameworks, libraries en concepten.
In plaats van losse proefprojecten verspreid over mijn computer te hebben, gebruik ik deze centrale repository om:

1. **Ervaring te bundelen** — alles in één monorepo, georganiseerd per omgeving (Frontend / Server).
2. **Sneller te refereren** — bij nieuwe projecten of jobs kan ik meteen zien *hoe ik iets eerder heb aangepakt*.
3. **Consistent te oefenen** — dezelfde database en basisopzet gebruiken om technologieën objectief te vergelijken.
4. **Mijn groei te documenteren** — wat ik leer, welke keuzes ik maak, en hoe ik ze technisch implementeer.

---

## 🏗️ Structuur (concept)

```
FullStackPlayground/
├─ Frontend/
│  ├─ web-next/         # Next.js (React + API routes)
│  ├─ web-vue/          # Vue 3 met Vite
│  └─ web-svelte/       # SvelteKit
│
├─ Server/
│  ├─ api-express/      # Node/Express REST API
│  ├─ api-fastapi/      # Python/FastAPI API
│  └─ api-php/          # PHP/Slim API
│
├─ packages/
│  └─ db/               # Prisma schema (gedeelde SQL database)
│
├─ docker-compose.yml   # Lokale PostgreSQL database via Docker
├─ .env.example
└─ README.md
```

---

## ⚙️ Technische doelen

| Domein              | Tools & Frameworks                                                  |
| ------------------- | ------------------------------------------------------------------- |
| **Frontend**        | Next.js, Vue, SvelteKit, HTML/CSS                                   |
| **Backend**         | Express (Node), FastAPI (Python), PHP (Slim)                        |
| **Database**        | PostgreSQL (via Docker Compose)                                     |
| **Infra & tooling** | pnpm workspaces, Turborepo (eventueel), Prisma ORM                  |
| **Doel**            | Eén monorepo met consistente codekwaliteit, linting en documentatie |

---

## 🚀 Toekomstige plannen

* Opzetten van een gedeelde lokale database met **Prisma + PostgreSQL**
* Basis REST API’s in Express en FastAPI
* Frontend prototypes met Next.js, Vue en SvelteKit
* CI/CD via GitHub Actions
* Documentatie van setups en leermomenten per onderdeel
* (Optioneel) Auth / OAuth integratie voor oefening

---

## 📘 Richtlijnen

* Alle projecten in deze monorepo dienen **educatieve doeleinden**.
* Geen commerciële of productiecode.
* Codevoorbeelden zijn vrij te gebruiken, verbeteren of uitbreiden.
* Ik houd de repository **publiek** om kennisdeling te stimuleren en om mijn leerproces transparant te maken.

---

## 🧩 Waarom een monorepo?

Een monorepo maakt het makkelijk om:

* Code te **delen** tussen projecten (bijv. via een shared `packages/` map).
* Frameworks **naast elkaar** te draaien en vergelijken.
* Een **centrale database** te gebruiken voor alle API’s.
* Sneller nieuwe experimenten op te zetten met minimale boilerplate.

---

## 💡 Filosofie

> “De beste manier om iets te leren, is het te bouwen — meerdere keren, op verschillende manieren.”

Deze repository is daar het bewijs van: geen eindproduct, maar een groeidocument van mijn ontwikkeling als full-stack developer.

---

## 📜 Licentie

Vrij te gebruiken, aanpassen en delen — zonder enige garantie.
