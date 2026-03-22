# Changelog

Alle vesentlige endringer i prosjektet er dokumentert her.
Format basert på [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [v1.6] — mars 2026
### Fikset
- Hamburger-knapp høyrejustert på mobil (var midtstilt)
- Kollapsbare dropdowns i mobilmenyen — underseksjoner vises kun ved trykk
- Pil roterer for å vise åpen/lukket tilstand

---

## [v1.5] — mars 2026
### Lagt til
- Apple-stil dropdown-meny på desktop: hover over Info, Verktøy og Spill gir undermeny
- Frosted glass-effekt på dropdown
- Usynlig bro mellom nav-lenke og dropdown så muspekeren ikke mister kontakt

---

## [v1.4] — mars 2026
### Endret
- Nav polert og README oppdatert

---

## [v1.3] — mars 2026
### Endret
- Koden i index.html forenklet og kommentert
- Fjernet død CSS (~30 linjer for nyheter-listestil)
- Spotlight-bakgrunner refaktorert med CSS-variabler
- Meny-funksjonene slått sammen
- Fjernet duplikat `history.scrollRestoration`

---

## [v1.2] — mars 2026
### Lagt til
- Versjonsstempel i footer
- Safari scroll-til-topp fix (double `requestAnimationFrame` i `pageshow`)
- Hjem-seksjon med kategorikort (Info, Verktøy, Spill)
- Ny navigasjon: 5 grupperte lenker i stedet for 10
- Gruppe-headers som scrollmål i siden
- Kontaktskjema-seksjon med backend (Node.js + Express, lagrer til JSON)

### Fikset
- Safari: siden landet alltid på "Skriving" ved refresh — nå alltid Hjem
- Safari: nav-lenker virket ikke (popstate-lytter fjernet)

---

## [v1.1] — februar/mars 2026
### Lagt til
- Snake-spill (Nokia-stil): 8-bit lyd, pause, top 3 highscore, wrap-around modus
- Kryssord-forbedringer: automatisk seiersjekk, statistikk per tema, tema-dropdown
- Navnefakta koblet til SSB live-API (antall, toppår, trend)
- SSB-ikoner i Apple SVG-stil
- Seksjon-spotlights (radial gradient-bakgrunn per seksjon)
- Hjem-ikon i nav

### Fikset
- Diverse Safari-scroll-bugs (flere iterasjoner)

---

## [v1.0] — januar/februar 2026
### Lagt til
- Apple-inspirert design: #f5f5f7 bakgrunn, #0071e3 aksent, frosted glass-nav
- Vær-seksjon med Open-Meteo API og canvas-animasjoner (regn, snø, sol, torden)
- Nyheter-seksjon med auto-refresh
- Analog klokke og skrivehastighetstест
- Kryssord med tema, timer og hint
- Tetris (lenke til eget spill)
- Mørk/lys-modus med SVG-toggle
- Mobilstøtte og responsivt design
- README
