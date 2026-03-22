# Changelog

Alle vesentlige endringer i prosjektet er dokumentert her.
Format basert på [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [v1.6] — 20. mars 2026
### Fikset
- Hamburger-knapp høyrejustert på mobil (var midtstilt)
- Kollapsbare dropdowns i mobilmenyen — underseksjoner vises kun ved trykk
- Pil roterer for å vise åpen/lukket tilstand

---

## [v1.5] — 20. mars 2026
### Lagt til
- Apple-stil dropdown-meny på desktop: hover over Info, Verktøy og Spill gir undermeny
- Frosted glass-effekt på dropdown
- Usynlig bro mellom nav-lenke og dropdown så muspekeren ikke mister kontakt

---

## [v1.4] — 20. mars 2026
### Endret
- Nav polert og README oppdatert

---

## [v1.3] — 19. mars 2026
### Endret
- Koden i index.html forenklet og kommentert
- Fjernet død CSS (~30 linjer for nyheter-listestil)
- Spotlight-bakgrunner refaktorert med CSS-variabler
- Meny-funksjonene slått sammen
- Fjernet duplikat `history.scrollRestoration`

---

## [v1.2] — 18. mars 2026
### Lagt til
- Versjonsstempel i footer
- Hjem-seksjon med kategorikort (Info, Verktøy, Spill)
- Ny navigasjon: 5 grupperte lenker i stedet for 10
- Gruppe-headers som scrollmål i siden
- Kontaktskjema-seksjon med backend (Node.js + Express, lagrer til JSON)
- Navnefakta koblet til SSB live-API (antall, toppår, trend)
- SSB-ikoner i Apple SVG-stil
- Seksjon-spotlights (radial gradient-bakgrunn per seksjon)

### Fikset
- Safari: siden landet alltid på "Skriving" ved refresh — nå alltid Hjem
- Safari: nav-lenker virket ikke (popstate-lytter fjernet)

---

## [v1.1] — 15. mars 2026
### Lagt til
- Snake-spill (Nokia-stil): 8-bit lyd, pause, top 3 highscore, wrap-around modus
- Kryssord med tema, timer, hint og automatisk seiersjekk
- Analog klokke og skrivehastighetstест
- Apple-inspirert design: større titler, mer luft, bedre animasjoner
- Mørk/lys-modus med SVG-toggle

---

## [v1.0] — 13–15. mars 2026
### Lagt til
- Første versjon av siden
- Vær-seksjon med Open-Meteo API og canvas-animasjoner (regn, snø, sol, torden)
- Nyheter-seksjon med auto-refresh
- Tetris (lenke til eget spill)
- Mobilstøtte og responsivt design
- README
