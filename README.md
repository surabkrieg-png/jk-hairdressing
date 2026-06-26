# JK Hairdressing - Static Website

Statische Website für JK Hairdressing by Jennifer Krieg, Friseursalon in Rostock.

## Über das Projekt

Dies ist eine statische HTML-Website, die WordPress ersetzt. Keine WordPress-Sicherheitslücken, kein Wartungsaufwand.

## Technologie

- **Frontend**: HTML5 + Tailwind CSS (CDN)
- **Hosting**: Cloudflare Pages
- **CI/CD**: GitHub Actions

## Struktur

```
/
├── index.html           # Startseite
├── impressum.html       # Impressum
├── datenschutz.html     # Datenschutzerklärung
├── blog/
│   ├── index.html       # Blog-Übersicht
│   ├── balayage-rostock/
│   │   └── index.html   # SEO-optimierter Artikel
│   └── brautstyling-rostock/
│       └── index.html   # SEO-optimierter Artikel
└── .github/
    └── workflows/
        └── deploy.yml   # Auto-Deployment
```

## SEO-Keywords

- Friseur Rostock
- Balayage Rostock
- Brautstyling Rostock
- Haarverlängerung Rostock
- Friseursalon Rostock

## Deployment

Automatisches Deployment bei Push auf `main` Branch via GitHub Actions zu Cloudflare Pages.

## Lokale Entwicklung

```bash
# Einfacher HTTP-Server
python3 -m http.server 8000

# Oder Live Server VS Code Extension
```

## Kontakt

Jennifer Krieg  
Wiener Platz 8  
18069 Rostock  
mail@jennifer-krieg.de