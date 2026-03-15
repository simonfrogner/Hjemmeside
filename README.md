# Simon sin stilige nettside

En personlig nettside vibe-kodet med [Claude Code](https://claude.ai/code).

🌐 **Live:** [simonfrogner.github.io/Hjemmeside](https://simonfrogner.github.io/Hjemmeside)

---

## Funksjoner

- **Hjem** — velkomstside med typewriter-effekt og konfetti ved navnegjetting
- **Navnefakta** — skriv inn navnet ditt og få morsomme fakta
- **Vær** — sanntidsvær basert på din posisjon med animerte væreffekter
- **Nyheter** — siste nyheter fra VG, auto-oppdateres hvert 5. minutt med lokal cache ved feil
- **Klokke** — analog og digital klokke med dato
- **Skriving** — skrivetesthurtigtest med WPM og nøyaktighetsstatistikk
- **Tetris** — klassisk Tetris med neon-design, musikk og highscore
- **Kryssord** — norsk kryssord med hint-system, tema-velger og highscore
- **Snake** — klassisk Nokia-spill med stigende vanskelighetsgrad og highscore
- **Mørkt tema** — bryter med SF Symbols-ikoner for å bytte mellom lyst og mørkt
- **Scroll-til-topp-knapp** — dukker opp når du scroller ned
- **Easter egg** — prøv å skrive «claude» i navnefeltet
- **Mobilstøtte** — responsivt design med hamburgermeny

## Design

Inspirert av Apples designspråk:

- Bakgrunn `#f5f5f7`, font `-apple-system`
- Frosted glass-navigasjonsbar
- Seksjonsetiketter og venstrestilte titler
- Myke overganger og animasjoner

## Teknologi

- Vanilla HTML / CSS / JavaScript
- [Open-Meteo API](https://open-meteo.com/) (vær, ingen API-nøkkel)
- Nominatim (omvendt geokoding)
- Canvas API (væranimasjoner)
- VG RSS via CORS-proxy med localStorage-cache
- Web Audio API (konfetti-lyd og Tetris-musikk)
- localStorage (tema og highscores)
- GitHub Pages (hosting)

---

Laget av [Simon Frogner](https://github.com/simonfrogner) med hjelp fra Claude Code
