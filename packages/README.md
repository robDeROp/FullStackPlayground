# Shared Packages

Gebruik deze map om code te delen tussen frontend- en backendprojecten. Denk aan:

- TypeScript types en interfaces
- UI component libraries (publiceerbaar via npm workspaces)
- Utility functies (bijv. datumformatting, logging)
- API clients of SDK's

## Aanpak

1. Maak subpackages aan via pnpm workspaces of npm workspaces.
2. Publiceer packages lokaal via `file:` of `workspace:` referenties.
3. Documenteer versiebeheer en breaking changes in `CHANGELOG.md` per package.

Houd gedeelde code framework-agnostisch zodat hergebruik eenvoudig blijft.
