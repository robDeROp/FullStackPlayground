# 🧩 FullStackPlayground

**FullStackPlayground** is mijn persoonlijke full-stack leeromgeving — een centrale plek waar ik experimenteer met verschillende **programmeertalen**, **frameworks** en **technologieën** om mijn vaardigheden als developer te verdiepen.

Het doel van dit project is om ervaring op te doen met uiteenlopende **frontend-** en **backend-omgevingen**, en om die kennis op een gestructureerde manier vast te leggen zodat ik ze later eenvoudig kan hergebruiken of als referentie kan raadplegen.

---

## 🎯 Doel van de repository

Deze monorepo dient als een **praktisch leerlab** waarin ik:

* Experimenteer met verschillende **web frameworks**
* Werk met diverse **programmeertalen**
* Oefen met **databasebeheer** via Docker
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

## 📁 Repository-structuur

```
.
├── frontend/
│   ├── shared/            # Framework-onafhankelijke UI-componenten en utilities
│   ├── vue-tailwind-typescript/
│   └── react-tailwind-typescript/
├── apis/
│   ├── express/
│   └── nestjs/
├── databases/
│   └── mysql/             # Docker-setup voor lokale MySQL
├── packages/              # Gedeelde code (types, utils, component libraries)
└── README.md
```

Elke map bevat een eigen `README.md` met setup- en startinstructies. Breid de structuur uit wanneer je nieuwe frameworks of tools wil testen.

---

## 📜 Licentie

Vrij te gebruiken, aanpassen en delen — zonder enige garantie.
