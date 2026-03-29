# Lessons Learned

## Navigasjon og layout
- Nav-underline (`::after`) vises feil på mobil pga. ulik padding — legg til `display: none` i mobile media query
- Hamburger X-knapp: `classList.toggle('åpen', undefined)` er upålitelig — sjekk alltid om klassen er tilstede eksplisitt
- Dropdown-pil-ikoner i nav bør fjernes — Simon liker ikke chevron-symboler

## Spill
- Pong delta-time: `sløyfe()` kallt fra `setTimeout` gir `ts=undefined` → `forrigeTs` blir `undefined` (ikke `null`) → NaN-bevegelse. Bruk `(!ts || forrigeTs === null) ? 1 : ...` og `forrigeTs = ts || null`
- Pong første frame: `dt=0` hvis `forrigeTs` settes til `ts` på første kall — returner `dt=1` når `forrigeTs === null`

## API og data
- Norsk Wikipedia (`no.wikipedia.org`) støtter ikke `onthisday` REST API-feeden — bruk `en.wikipedia.org`
- MyMemory oversettings-API er upålitelig og langsomt for live bruk — unngå automatisk oversetting av Wikipedia-hendelser

## Animasjoner
- Simon likte ikke animasjonspakken som ble implementert i v1.16 — den ble rullet tilbake. Vær forsiktig med store animasjonsendringer
- Hjem-kort: store ikoner med puste-animasjon og farget glow ved hover foretrekkes fremfor beskrivelsestekst

## Generelle regler
- Oppdater alltid hjem-kortbeskrivelser når nye seksjoner legges til under Info/Verktøy/Spill
- Oppdater alltid versjonsstempel i footer og README.md før push
- Aldri push uten å spørre Simon først
