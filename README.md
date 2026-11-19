# GunplaLog – kostenlose iPhone-Web-App

Deutsche, offlinefähige PWA für Gunpla-Projekte. Keine Apple-Developer-Mitgliedschaft und kein Xcode nötig.

## Enthalten
- Projektübersicht und neue Projekte
- Baufortschritt mit 10 frei abhakbaren Phasen
- Bautimer mit Start, Pause und Speichern von Sitzungen
- Bautagebuch
- Farben-, Werkzeug- und Materialinventar
- Sammlung
- JSON-Datensicherung exportieren/importieren
- Service Worker für Offline-App-Shell

## Auf dem iPhone verwenden
1. Die Dateien auf einen HTTPS-Webhost hochladen (z. B. GitHub Pages).
2. Die veröffentlichte Adresse in **Safari** öffnen.
3. Teilen → **Zum Home-Bildschirm**.
4. **Als Web-App öffnen** aktivieren (falls angezeigt) → Hinzufügen.
5. App einmal bei bestehender Verbindung starten, damit die Offline-Dateien gecacht werden.

Danach sind die Kernfunktionen ohne Internet nutzbar. Service Worker benötigen HTTPS (localhost ausgenommen).

## Hinweis zum aktuellen Entwicklungsstand
Dies ist ein funktionsfähiger Starter-Prototyp, keine native App-Store-App. Daten liegen lokal im Browser-Speicher des Geräts. Browserdaten löschen kann lokale Daten entfernen – daher regelmäßig unter Einstellungen eine Sicherung exportieren. Timer-Zeit wird bei App-Neustart anhand des gespeicherten Zeitstempels berechnet; iOS garantiert keine dauerhaft laufende Hintergrundausführung oder Live-Aktualisierung bei geschlossener App. Fotos, Cloud-Sync, Push-Nachrichten und Community sind noch nicht implementiert.
