# BIM4ALL Academie — website-export

Complete, werkende export van de BIM4ALL Academie-website (25 pagina's, responsive).

## Gebruik
Statische site — geen build-stap nodig. Serveer de map via een webserver, bijv.:

    npx serve .

Startpagina: `BIM4ALL Homepage v2.dc.html`. Direct openen vanaf schijf werkt niet overal (fetch van support.js vereist http).

## Inhoud
- `*.dc.html` — alle pagina's (Nav.dc.html en Footer.dc.html zijn gedeelde componenten, geladen door de pagina's)
- `support.js` — runtime die de pagina's rendert (vereist)
- `image-slot.js` — component voor foto-slots (vereist)
- `logo.png`, `assets/` — beelden en logo's

## Voor livegang (developer-checklist)
- HTTPS afdwingen
- Contactformulier: server-side afhandeling met spam- en injectiebescherming (nu prototype, verstuurt niets)
- AVG: cookiemelding indien tracking, verwerking persoonsgegevens checken
- Security headers (CSP, X-Frame-Options, etc.)
- Nette URL's/redirects (bijv. `/leeraanbod` → `Leeraanbod.dc.html`)
