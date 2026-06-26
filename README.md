# JK Hairdressing - Static Website

Statische Website für JK Hairdressing by Jennifer Krieg, Friseursalon in Rostock.

## Über das Projekt

Dies ist eine statische HTML-Website, die WordPress ersetzt. Keine WordPress-Sicherheitslücken, kein Wartungsaufwand.

## Technologie

- **Frontend**: HTML5 + Tailwind CSS (CDN)
- **Icons**: Inline SVG
- **Buchung**: Salonized Widget (`salonized-loader.js`)
- **Preise**: Salonized iframe (`jennifer-krieg-jk.salonized.com/services?layout=embed`)
- **Hosting**: Cloudflare Pages
- **CI/CD**: GitHub Actions

## Struktur

```
/
├── index.html              # Startseite
├── impressum.html          # Impressum
├── datenschutz.html        # Datenschutzerklärung
├── salonized-loader.js     # Salonized Buchungs-Button
├── images/                 # Lokale Bilder
├── blog/
│   ├── index.html          # Blog-Übersicht
│   ├── posts.json          # Blog-Daten
│   └── images/             # Blog-Bilder
├── balayage-rostock/       # SEO Landing Page
├── brautstyling-rostock/   # SEO Landing Page
├── haarverdichtung-rostock/# SEO Landing Page
└── .github/workflows/
    └── deploy.yml          # Auto-Deployment zu Cloudflare Pages
```

## SEO-Keywords

- Friseur Rostock
- Balayage Rostock
- Brautstyling Rostock
- Haarverdichtung Rostock
- Friseursalon Rostock

## Deployment

Automatisches Deployment bei Push auf `main` Branch via GitHub Actions zu Cloudflare Pages.

Benötigte GitHub Secrets:
- `CLOUDFLARE_API_TOKEN`
- `CLOUDFLARE_ACCOUNT_ID`

## Lokale Entwicklung

```bash
cd /path/to/repo
python3 -m http.server 8080
```

## Kontakt

Jennifer Krieg  
Wiener Platz 8  
18069 Rostock  
mail@jennifer-krieg.de
