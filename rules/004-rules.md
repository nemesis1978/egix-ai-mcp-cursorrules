---
description: Regole guida per l'uso dell’AI nei progetti con Cursor, Streamlit, TRAE
globs: ["**/*.ts", "**/*.tsx", "**/*.py", "**/*.md"]
---

## Linguaggio di default

- Se non viene specificato:
  - Usa TypeScript per web
  - Usa Python per backend/automazioni
  - Usa Flutter o React Native per mobile
  - Usa Electron o Tkinter per desktop

## Quando il linguaggio non è specificato:

- Cerca la regola migliore tra:
  - `004-rules.md` per default
  - `003-prompts.md` per suggerimenti interattivi
  - file extra nella cartella `rules/awesome/` (se esistono)

- Se trovi una regola esistente per il contesto, applicala.
- Se non esiste, scegli lo stack più leggero, sicuro e mantenibile.

## Obblighi AI

- Non riscrivere file se non richiesto
- Refactor solo se migliora modularità o leggibilità
- Non duplicare codice

## Testing

- Usa `pytest` per Python
- Scrivi sempre: test normale + edge case + errore previsto
- Mocka API esterne

## UI/UX

- Per Streamlit o Web, separa logica da interfaccia
- Scrivi codice pulito, commentato, moderno
