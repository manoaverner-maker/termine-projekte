# Termine & Projekte

Persönliche Terminübersicht für Lüftungsprojekte — eine schlanke, offline-fähige Web-App ohne Build-Schritt und ohne Abhängigkeiten (Vanilla HTML/CSS/JS).

## Was sie kann

- **Nächste Termine**: die 4 nächsten Termine über alle Projekte, aufklappbar auf alle.
- **Projekte** als Accordion mit freiem Infofeld (speichert beim Tippen), Terminen und Notizen im Chat-Stil.
- **5 Terminarten** mit fester Farbcodierung: Start / Klärung, Planung, Beschaffung, Montage, Abschluss.
- **Live-Countdown** pro Termin: `3T 04Std` ab 1 Tag, `HH:MM` (rot) unter 24 Std, `Überfällig` (rot) nach Ablauf — aktualisiert sich automatisch.
- **Kein endgültiges Löschen**: Termine werden archiviert, Notizen als gelöscht markiert — beides jederzeit wiederherstellbar.
- **Backup**: Daten als JSON exportieren/importieren (Links am Seitenende).

## Daten

Alles liegt lokal im Browser (`localStorage`, Schlüssel `termine_v1`). Kein Backend, kein Login. Beim Import wird der bisherige Stand automatisch im Browser gesichert.

## Nutzung

- Direkt `index.html` öffnen, oder
- über GitHub Pages aufrufen und als **PWA installieren** (im Browser-Menü «Zum Startbildschirm hinzufügen» / «App installieren») — funktioniert danach auch offline.

## Lokale Vorschau

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1
# → http://localhost:8126/
```
