# Simon sin stilige nettside

En personlig nettside laget med [Claude Code](https://claude.ai/code).

🌐 **Live:** [simonfrogner.github.io/Hjemmeside](https://simonfrogner.github.io/Hjemmeside)

---

## Funksjoner

Navigasjonen er gruppert i fem seksjoner:

**Hjem** — velkomstside med kategorikort som lenker til Info, Verktøy og Spill

**Info**
- Vær — sanntidsvær basert på din posisjon eller by, med animerte væreffekter og 7-dagers prognose
- Nyheter — siste nyheter fra VG, auto-oppdateres hvert 5. minutt med lokal cache ved feil
- Boligpriser — interaktiv graf med SSB-data, søk på kommune, togglebare serier
- Fjelloverganger — oversikt over 10 norske fjelloverganger med høyde og riksvegnummer

**Verktøy**
- Klokke — analog og digital klokke med dato
- Skriving — skrivehurtigtest med WPM og nøyaktighetsstatistikk
- Navnefakta — skriv inn navnet ditt og få live data fra SSB (antall, toppår, trend) samt morsomme fakta

**Spill**
- Kryssord — norsk kryssord med hint-system, ordavsløring, auto-deteksjon av seier, statistikk og nedtrekksmeny for temavalg
- Tetris — klassisk Tetris med neon-design, musikk, nivåstigning og highscore
- Snake — klassisk Nokia-spill med LCD-farger, pause, 8-bit lyd, wrap-around modus og top 3 highscore
- Memory — 4×4 emoji-memory med flip-animasjon, lydeffekter, konfetti, beste rekord og 2-spiller modus

**Kontakt** — kontaktskjema

**Generelt**
- Mørkt tema — bryter med SF Symbols-ikoner for å bytte mellom lyst og mørkt, synkroniseres til alle spill
- Fade-overgang — nav-lenker fader siden ut/inn istedenfor å scrolle
- Scroll-til-topp-knapp — dukker opp når du scroller ned
- Easter egg — prøv å skrive «claude» i navnefeltet
- Mobilstøtte — responsivt design med hamburgermeny

## Design

Inspirert av Apples designspråk:

- Bakgrunn `#f5f5f7`, font `-apple-system`
- Frosted glass-navigasjonsbar, midtstilt, med Apple-favicon (blå sirkel med S)
- Apple-stil dropdown-meny på desktop: hover over Info, Verktøy og Spill
- Kollapsbar mobilmeny med nedtrekkbare underseksjoner
- Radial spotlight-bakgrunn med unik farge per seksjon
- Seksjonsetiketter og venstrestilte titler
- Myke overganger og animasjoner

## Teknologi

- Vanilla HTML / CSS / JavaScript
- [Open-Meteo API](https://open-meteo.com/) (vær, ingen API-nøkkel)
- [SSB PxWeb API](https://data.ssb.no/) (navnestatistikk, ingen API-nøkkel)
- Nominatim (omvendt geokoding)
- Canvas API (væranimasjoner, Snake-spill, boligpris-graf, konfetti)
- VG RSS via CORS-proxy med localStorage-cache
- Web Audio API (Memory-lydeffekter, Tetris-musikk og Snake-lydeffekter)
- localStorage (tema, highscores, rekorder og statistikk)
- SSB PxWeb API (boligpriser tabell 06035, kvadratmeterpris)
- GitHub Pages (hosting)

---

Laget av [Simon Frogner](https://github.com/simonfrogner) med hjelp fra Claude Code
