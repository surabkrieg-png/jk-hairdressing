# JK Hairdressing - Static Website

Statische HTML-Website für JK Hairdressing by Jennifer Krieg, Friseursalon in Rostock.

## Über das Projekt

Dies ist ein 1:1 statischer Nachbau der bestehenden WordPress-Website (`jennifer-krieg.de`), um WordPress-Sicherheitslücken und Wartungsaufwand zu vermeiden.

## Technologie

- **Frontend**: HTML5 + Tailwind CSS (CDN)
- **Icons**: Inline SVG
- **Buchung**: Salonized Widget
- **Preisliste**: Salonized iframe (`jennifer-krieg-jk.salonized.com/services?layout=embed`)
- **Bewertungen**: Salonized Reviews Mini Widget + Link zu Google-Bewertungen
- **Hosting**: Cloudflare Pages
- **CI/CD**: GitHub Actions

## Struktur

```
/
├── index.html              # Startseite
├── impressum.html          # Impressum
├── datenschutz.html        # Datenschutzerklärung
├── blog/index.html         # Blog-Übersicht
├── images/                 # Lokale Bilder
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
cd /root/Claude-Code-Workspace/Projekte/jennifer-krieg-website
python3 -m http.server 8080
```

## Kontakt

Jennifer Krieg  
Wiener Platz 8  
18069 Rostock  
mail@jennifer-krieg.de
