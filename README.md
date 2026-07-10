# Vindfall — landningssida

Landningssidan för vindfall.se, byggd i Claude Design (React-bundle,
fristående — bilderna ligger inbäddade i index.html som base64).
Publiceras via GitHub Pages från detta repo.

## Struktur

- `index.html` — hela sidan (exporterad "standalone" från Claude Design)
- `bilder/` — HELA mockupbanken i full upplösning, kategorisorterad
  (iphone/, macbook/, desktop/, kort/, billboards/, stickers/, skyltar/,
  posters/) — används när vi byter vilka bilder sidan visar

## Byta bilder på sidan

Sidans foton är inbäddade i bundlen. Två vägar:
1. Be Claude Code byta — den patchar base64-blocken mot valda filer ur
   `bilder/` (eller refererar dem relativt).
2. Gör om i Claude Design och exportera ny standalone → ersätt index.html.

## Deploy

Pushas till `main` → GitHub Pages publicerar automatiskt.
