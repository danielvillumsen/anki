# FlashDeck 🧠

En Anki-inspireret spaced repetition app — én enkelt HTML-fil, der virker direkte i browseren på telefon og computer. Alle data gemmes lokalt i browseren (localStorage).

## Kom i gang

### Åbn lokalt
Dobbeltklik på `flashdeck.html` — den åbner i din browser med 151 Pandora-flashcards klar til brug.

### GitHub Pages (anbefalet til mobil)

1. Opret et nyt repository på GitHub (f.eks. `flashdeck`)
2. Upload `flashdeck.html` og omdøb den til `index.html`
3. Gå til **Settings → Pages → Source: main branch / root**
4. Din app er nu tilgængelig på `https://[dit-brugernavn].github.io/flashdeck`
5. Åbn linket på din telefon og tilføj til hjemskærmen (iOS: Del → Føj til hjemskærm)

## Funktioner

- **151 Pandora-flashcards** forudindlæst (HA-opgave om aktieanalyse)
- **SM-2 algoritme** — viser kort præcis når du er ved at glemme dem
- **Kort-flip animation** — tryk på kortet for at se svaret
- **Bedømmelsesknapper** med interval-forhåndsvisning (Igen / Svær / God / Let)
- **Tastaturstenveje**: Space/Enter = flip, 1-4 = bedøm
- **Importer TSV-filer** — tilføj egne kort fra Anki-eksport
- **Statistik** — streak, forecast og review-oversigt
- **Søg og gennemse** alle kort
- **Tilføj/redigér** kort og decks
- Virker offline efter første indlæsning

## TSV-import format

```
Spørgsmål[TAB]Svar
```
eller (med Anki-eksport):
```
nummer[TAB]Spørgsmål[TAB]Svar
```

## SM-2 algoritmen kort fortalt

| Knap | Ny/Lær | Review |
|------|--------|--------|
| Igen | 1 min  | 10 min, let interval |
| Svær | næste trin | interval × 1.2 |
| God  | dimitterer (1 dag) | interval × ease |
| Let  | dimitterer (4 dage) | interval × ease × 1.3 |
