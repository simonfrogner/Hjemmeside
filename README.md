# Simon sin stilige nettside

En personlig nettside laget med [Claude Code](https://claude.ai/code).

🌐 **Live:** [simonfrogner.github.io/Hjemmeside](https://simonfrogner.github.io/Hjemmeside)

---

## Funksjoner

Navigasjonen er gruppert i fem seksjoner:

**Hjem** — velkomstside med animert gradient-bakgrunn og kategorikort (Info, Verktøy, Spill) med bounce-animasjon ved hover

**Info**
- Klokke — analog og digital klokke med dato
- Tidssoner — mini-analogklokker med digital tid for 8 byer rundt om i verden, oppdateres hvert sekund
- Vær — sanntidsvær basert på din posisjon eller by, med animerte væreffekter og 7-dagers prognose
- Nyheter — siste nyheter fra NRK, VG og E24 med tab-velger, auto-oppdateres hvert 5. minutt med lokal cache ved feil
- Boligpriser — interaktiv graf med SSB-data, søk på kommune, togglebare serier
- Strømpriser — 24-timers stolpediagram med hover-tooltip, snitt/min/maks og regionvelger (NO1–NO5)
- Valuta — kurser for EUR, USD, GBP, SEK og DKK mot NOK med omregner og kursendring fra forrige dag
- Navnefakta — skriv inn navnet ditt og få live data fra SSB (antall, toppår, trend) samt morsomme fakta
- I dag i historien — 8 tilfeldige historiske hendelser fra Wikipedia for dagens dato

**Verktøy**
- Skriving — skrivehurtigtest med WPM og nøyaktighetsstatistikk
- Nedtelling — legg til hendelser med dato og se dager igjen med fargekodet fremgangsbjelke; egen fane for norske helligdager med neste kommende uthevet
- Kalkulator — Apple-stil kalkulator med historikk (siste 10 beregninger), kopier resultat og tastaturstøtte

**Spill**
- Pong — klassisk arkadespill mot AI (3 vanskelighetsgrader, dynamisk AI) eller 2-spiller på samme enhet; konfetti ved seier, lyd, mobilstøtte
- Tetris — klassisk Tetris med neon-design, musikk, nivåstigning og highscore
- Snake — klassisk Nokia-spill med LCD-farger, pause, 8-bit lyd, wrap-around modus og top 3 highscore
- Memory — 4×4 emoji-memory med flip-animasjon, lydeffekter, konfetti, beste rekord og 2-spiller modus
- Kryssord — norsk kryssord med hint-system, ordavsløring, auto-deteksjon av seier, statistikk og nedtrekksmeny for temavalg

**Kontakt** — kontaktskjema

**Generelt**
- Mørkt tema — bryter med SF Symbols-ikoner for å bytte mellom lyst og mørkt, synkroniseres til alle spill
- Fade-overgang — nav-lenker fader siden ut/inn istedenfor å scrolle
- Scroll-til-topp-knapp — dukker opp når du scroller ned
- Easter egg — prøv å skrive «claude» i navnefeltet
- Mobilstøtte — responsivt design med hamburgermeny

## Versjon

v1.19 — Hamburger-meny fikset, «Historie» etikett, hjem-kort uten beskrivelse

## Design

Inspirert av Apples designspråk:

- Bakgrunn `#f5f5f7`, font `-apple-system`
- Animert gradient-bakgrunn på hjem-siden (lilla/blå/rosa)
- Frosted glass-kategorikort med bounce-animasjon på hjem-siden
- Frosted glass-navigasjonsbar, midtstilt, med Apple-favicon (blå sirkel med S)
- Apple-stil dropdown-meny på desktop: hover over Info, Verktøy og Spill
- Kollapsbar mobilmeny med nedtrekkbare underseksjoner
- Radial spotlight-bakgrunn med unik farge per seksjon
- Seksjonsetiketter og venstrestilte titler
- Myke overganger og animasjoner

## Teknologi

- Vanilla HTML / CSS / JavaScript
- [Open-Meteo API](https://open-meteo.com/) (vær, ingen API-nøkkel)
- [SSB PxWeb API](https://data.ssb.no/) (navnestatistikk og boligpriser, ingen API-nøkkel)
- [Norges Bank API](https://data.norges-bank.no/) (valutakurser, ingen API-nøkkel)
- [hvakosterstrommen.no API](https://www.hvakosterstrommen.no/strompris-api) (strømpriser, ingen API-nøkkel)
- [Nager.Date API](https://date.nager.at/) (norske helligdager, ingen API-nøkkel)
- NRK, VG og E24 RSS via CORS-proxy med localStorage-cache per kilde
- Nominatim (omvendt geokoding)
- Canvas API (væranimasjoner, Snake-spill, boligpris-graf, strømpris-graf, konfetti)
- Web Audio API (Memory-lydeffekter, Tetris-musikk og Snake-lydeffekter)
- localStorage (tema, highscores, rekorder, nedtellinger og statistikk)
- GitHub Pages (hosting)

---

Laget av [Simon Frogner](https://github.com/simonfrogner) med hjelp fra Claude Code
