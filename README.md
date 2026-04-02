# Notfallkarte PWA – Deployment

## Einfachster Weg: GitHub Pages

1. **GitHub-Repo erstellen** (z.B. `notfallkarte`)
2. Alle Dateien aus diesem Ordner ins Repo pushen:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-180.png`
   - `icon-192.png`
   - `icon-512.png`
   - `icon-1024.png`
   - `icon-152.png`
3. **Settings → Pages → Source: main branch** aktivieren
4. URL wird: `https://DEINNAME.github.io/notfallkarte/`

## Auf dem iPhone installieren

1. URL in **Safari** öffnen (nicht Chrome!)
2. **Teilen-Button** (□↑) antippen
3. **Zum Home-Bildschirm** wählen
4. Fertig – App-Icon erscheint, öffnet sich fullscreen, funktioniert offline

## Alternative: Glitch.com

1. Neues Projekt auf glitch.com erstellen
2. Alle Dateien hochladen
3. URL direkt in Safari öffnen und zum Home-Bildschirm hinzufügen

## Enthaltene Dateien

| Datei | Zweck |
|-------|-------|
| index.html | Die komplette App (self-contained) |
| manifest.json | PWA-Manifest (Name, Icons, Display-Modus) |
| sw.js | Service Worker für Offline-Betrieb |
| icon-*.png | App-Icons in verschiedenen Größen |

## Hinweise

- Die App läuft **komplett offline** nach dem ersten Laden
- Kein Ablaufdatum, kein Developer Account nötig
- Update: einfach neue `index.html` ins Repo pushen, `CACHE_NAME` in `sw.js` hochzählen (z.B. `notfallkarte-v2`)
