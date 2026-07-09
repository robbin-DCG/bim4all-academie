# BIM4ALL Academie — website (eerste concept)

Statische website voor de BIM4ALL Academie: leren & ontwikkelen, consulting en AI voor de bouwsector.

## Structuur
- `BIM4ALL Homepage v2.dc.html` — startpagina (open deze als index)
- Overige `*.dc.html` — pagina's; `Nav.dc.html` en `Footer.dc.html` zijn gedeelde componenten
- `Training.dc.html?t=<slug>` — detailpagina per klassikale training
- `Artikel.dc.html?a=<slug>` — detailpagina per kennisartikel
- `support.js` + `image-slot.js` — runtime (vereist)
- `assets/` — beelden en logo's

## Lokaal bekijken / hosten
De site is volledig statisch. Serveer de map met een webserver (bestanden openen via `file://` werkt niet door de componentimports), bijvoorbeeld:

```bash
npx serve .
# of
python3 -m http.server 8000
```

Open daarna `BIM4ALL Homepage v2.dc.html`.

## Nog open (eerste concept)
- Agenda-boekingslink op Contact ("Plan direct in de agenda")
- Startdata trainingen en resultaatcijfers klantverhalen controleren
- Formulieren zijn nog niet gekoppeld aan een backend/mailservice
- Aanmelden trainingen verloopt straks via Plusport
