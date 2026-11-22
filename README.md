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


## iPhone Duo Navigation
Wiederhergestellte Duo-Anpassung: kompakte untere Navigation auf beiden Displays, keine seitliche Symbolleiste und keine Positionsregler.


## Cinematic HUD Update
Animierte HUD-Panels, Seitenwechsel, Lichtreflexe, Fortschrittsanzeigen, Timer-Ringe und Navigations-Highlights. Die Duo-Navigation bleibt unten. `prefers-reduced-motion` deaktiviert dekorative Animationen.


## Liquid Glass Edition
Apple-Liquid-Glass-inspirierte PWA-Oberfläche mit Glasnavigation unten, stärkerer Tiefe und zugänglichen Transparenz-/Bewegungs-Fallbacks. Siehe TESTBERICHT.md.


## Werkzeugverwaltung
Werkzeuge und Farben lassen sich jetzt getrennt anlegen, bearbeiten und nach Bestätigung löschen. Bestehende Einträge bleiben erhalten.


## Liquid Motion Edition
Deutlich verstärkte CSS-Animationen: gestaffelte Seiten-/Kartenauftritte, dynamisches Glaslicht, animierte Navigation, Timer-Aura, Lade-/Fortschrittsglanz, pulsierende Statusanzeigen. Bei aktivierter iOS-Einstellung »Bewegung reduzieren« sind die Animationen deaktiviert. Werkzeugverwaltung aus der vorigen Version bleibt erhalten.


## Neue Projektkategorien
Modellmaßstab: 30MS, 30MM, 30MF, PokePla. Grade: FRM, FRS. Alle bisherigen Optionen bleiben erhalten; bereits gespeicherte Werte werden beim Bearbeiten weiter angezeigt.


## Modellreihen (v15)
Neues Projektfeld „Modellreihe“ mit Gunpla, 30MS, 30MM, 30MF, PokePla, Sonstige. Maßstab enthält nur echte Maßstabswerte. FRM/FRS bleiben Grades. Alte als Maßstab gespeicherte Modellreihen werden beim Laden in das neue Feld übernommen. Projektkarten, Detailansicht, Dashboard, Hangar, Timer und Suche zeigen bzw. berücksichtigen Modellreihen.
