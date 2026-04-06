# Jörg Martin - Digitale Entlastung

Statische Website fuer das Angebot "Digitale Entlastung" mit Fokus auf kleine Handwerksbetriebe.

## Aktueller Stand

- Alle Seiten live und konsistent verlinkt.
- Favicon-Setup bereinigt (inkl. Dark-Variante und Manifest).
- Social-Links auf allen Seiten vereinheitlicht.
- OG/Twitter-Metadaten auf allen Seiten konsistent.
- Dediziertes Social-Preview-Bild vorhanden: `assets/og-image.jpg` (1200x630).
- Kontaktseite bereinigt: keine Inline-Styles/Inline-Hover-Events mehr.
- Performance-Optimierungen umgesetzt:
  - `assets/portrait.jpg` stark komprimiert (Fallback-Bild).
  - `ueber-mich.html` nutzt WebP mit JPG-Fallback (`picture`).
  - `assets/logo.png` deutlich verkleinert fuer schnelleren Seitenaufbau.
- Unnoetiges Asset entfernt (`assets/portrait-rund.png`).

## Technik

- HTML, CSS, JavaScript (ohne Framework).
- Einheitliches Script-Loading mit `assets/script.js` via `defer`.
- Strukturierte Daten ueber JSON-LD.

## Seiten

- `index.html`
- `leistungen.html`
- `ueber-mich.html`
- `zertifikate.html`
- `kontakt.html`
- `impressum.html`
- `datenschutz.html`
- `404.html`

## SEO und Sharing

- Canonicals sind derzeit auf `https://joergmartindigital.de` gesetzt (aktueller Live-Stand).
- `robots.txt`, `sitemap.xml` und `site.webmanifest` sind vorhanden.
- Open Graph und Twitter Cards verweisen auf `assets/og-image.jpg`.

## Deployment und Pflege

1. Aenderungen lokal committen und nach `main` pushen.
2. Nach groesseren Meta- oder Bildaenderungen Social-Preview einmal neu validieren.
3. Regelmaessig kurz pruefen:
   - interne Links
   - externe Kernlinks (Forms, Social)
   - Dateigroessen grosser Assets

## Naechste sinnvolle Schritte

1. Domain-Umstellung erst nach Live-Schaltung der neuen Domain:
   - Canonicals, Sitemap, Robots, OG/Twitter, JSON-LD auf Ziel-Domain umstellen.
   - 301-Redirect-Konzept von Alt- auf Zieldomain.
2. Optional: weiterer Accessibility-Pass (Kontraste, Fokusfuehrung, Formulare).
3. Optional: Lighthouse-Benchmark dokumentieren (vorher/nachher).

