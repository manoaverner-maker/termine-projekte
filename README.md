# Termine & Projekte

Persönliche Terminübersicht für Lüftungsprojekte — eine schlanke, offline-fähige Web-App ohne Build-Schritt und ohne Abhängigkeiten (Vanilla HTML/CSS/JS).

## Was sie kann

- **Nächste Termine**: die 4 nächsten Termine über alle Projekte, gruppiert nach Überfällig / Heute / Morgen / Später, aufklappbar auf alle.
- **Abhaken direkt in der Liste**: Häkchen-Button archiviert den Termin mit Animation — ohne Umweg übers Projekt.
- **Projekte** als Accordion mit freiem Infofeld (speichert beim Tippen), Terminen und Notizen im Chat-Stil. Fertige Projekte lassen sich abschliessen (und wiederherstellen).
- **Termine bearbeiten**: Tippen auf einen Termin öffnet das vorbefüllte Formular.
- **In Kalender übernehmen**: pro Termin eine `.ics`-Datei mit Erinnerungen (1 Tag und 1 Std vorher) für Outlook/Handy-Kalender — so klingelt es auch, wenn die App zu ist.
- **5 Terminarten** mit fester Farbcodierung: Start / Klärung, Planung, Beschaffung, Montage, Abschluss.
- **Montage-Termine** mit Zusatzangaben: Monteur sowie beliebig viele Lieferungen (Lieferant + Ankunft, je mit eigenem Countdown).
- **Objekt & Kontakte** pro Projekt: Adresse mit Google-Maps-Knopf, Kontakte (Bauleitung, Elektriker, …) mit Direktanruf-Link.
- **Live-Timer** pro Termin, sekündlich tickend mit Stoppuhr-Symbol: `3T 04:12:33` ab 1 Tag, `HH:MM:SS` (rot) unter 24 Std, `Überfällig` (rot, pulsierend) nach Ablauf.
- **Dark Mode**: automatisch nach Systemeinstellung, umschaltbar im Header (Automatisch / Dunkel / Hell).
- **Kein endgültiges Löschen**: Termine werden archiviert, Notizen als gelöscht markiert — beides jederzeit wiederherstellbar.
- **Backup**: Daten als JSON exportieren/importieren (Links am Seitenende). Der Import **führt zusammen** statt zu ersetzen — bei Konflikten gewinnt der neuere Stand, gelöscht wird nichts; so lässt sich auch zwischen Handy und PC abgleichen.

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
