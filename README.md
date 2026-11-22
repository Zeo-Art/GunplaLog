# GunplaLog – TRON Command Center

Kostenloser, deutschsprachiger Gunpla-Tracker als installierbare Web-App (PWA).

## Enthaltene Funktionen
- Kommandozentrale mit persönlicher Begrüßung und aktivem Projekt
- Projekte/Modelle anlegen, bearbeiten, löschen und als aktiv markieren
- Hangar mit kompakten anklickbaren Modellkarten und Detailansicht
- Modellgrade und Maßstäbe 1/100, 1/144, 1/60, 1/35
- Modellbild lokal hinterlegen
- Bauschritte und automatischer Fortschritt
- Bauzeittimer mit gespeicherten Sitzungen, Datum und Gesamtbauzeit
- Bautagebuch
- Paint Lab und Werkzeug-/Materialinventar
- Profil mit Benutzername, Avatar und Kurzbeschreibung
- JSON-Export und -Import
- Offline-App-Shell via Service Worker
- Responsives Layout für Hoch-/Querformat und schmale/breite Displays

## Installation
1. Dateien auf einen HTTPS-Webhost laden (z. B. GitHub Pages mit öffentlichem Repository).
2. URL in Safari auf dem iPhone öffnen.
3. Teilen → „Zum Home-Bildschirm“.
4. App einmal online öffnen, damit die Offline-Dateien zwischengespeichert werden.

## Wichtige Hinweise
- Daten werden lokal im Browser (localStorage) gespeichert. Browserdaten löschen kann Daten entfernen. Regelmäßig JSON-Backups exportieren.
- Für Offline-Cache und PWA-Installation wird HTTPS benötigt (localhost ausgenommen).
- Der Timer berechnet die Zeit über gespeicherte Zeitstempel. iOS garantiert keine dauerhafte Hintergrundausführung oder Live-Aktualisierung im Hintergrund. Beim erneuten Öffnen wird die verstrichene Zeit berechnet.
- Modellbilder werden lokal im Browser gespeichert; große Bilder werden beim Import verkleinert.
- Dieses Paket ist ein funktionsfähiger Prototyp, keine native iOS-App. Es enthält keine Cloud-Synchronisierung, Accounts oder Push-Benachrichtigungen.
- Die App verwendet für ihre Oberfläche keine externen Laufzeitdienste. Die optionale Google-Font-Einbindung kann offline nicht geladen werden; System-Fallbacks greifen.


## Update: Navigation und Projekt-Detailansicht
- Feste untere Navigation mit fünf Symbolen: Home, Projekte, Timer, Hangar und Mehr.
- Tagebuch, Paint Lab, Werkzeuge, Profil und Einstellungen sind über „Mehr“ erreichbar.
- Event-Bindings werden nach dem Erzeugen der Projekt-Detailansicht und des Projektformulars erneut gesetzt; Schließen, Bearbeiten, Löschen und Bauschritt-Aktionen sind dadurch erreichbar.


## Neue Version
Projekt-/Hangar-Trennung, Suchfelder, größeres festes Bottom-Menü, Timer-Fix, Tagebuch-Bearbeitung und Profilbild im Dashboard. Siehe TESTBERICHT.md für die Grenzen der Prüfungen.


## iPhone Duo
Responsive Anpassung fuer das 5,4-Zoll-Aussendisplay und das 7,6-Zoll-Innendisplay. Passt sich beim Auf- und Zuklappen sowie bei Rotation und Split View an den jeweils verfuegbaren Viewport an. TRON-Design und bestehende Datenstruktur bleiben erhalten.
