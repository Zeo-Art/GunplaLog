# GunplaLog – Prüfbericht zur neuen Version

## Umgesetzte Änderungen
- Timer: Start und Stopp verwenden jetzt das aktive Projekt; Stop speichert eine Sitzung.
- Projekte: nur offene Projekte, aktives Projekt zuerst, Suche nach Name/Serie/Grade/Maßstab.
- Hangar: nur abgeschlossene Modelle, Suche; Modelle können über die Detailansicht wieder geöffnet werden.
- Projekt-Detailansicht: Abschluss-/Wiederöffnen-Schaltfläche, vorhandene Bearbeiten-/Löschen- und Bauschrittaktionen.
- Bautagebuch: Einträge bearbeiten (Text und Datum) und löschen.
- Kommandozentrale: Profilbild mit Neon-Rahmen.
- Navigation: fünf große Symbole, fest am unteren Bildschirmrand, Safe-Area-Abstand.
- Service-Worker-Cache auf Version 3 aktualisiert.

## Durchgeführte Prüfungen
- ZIP-Dateien und erwartete App-Dateien geprüft.
- 17 statische Prüfungen: alle bestanden.
- JavaScript-Syntaxprüfung mit Node.js: bestanden.
- HTML-Seiten und Navigationsstruktur geprüft.

## Nicht als bestanden behauptet
Die vollständige interaktive Browserprüfung konnte nicht ausgeführt werden: Der Testbrowser blockiert das Laden lokaler Dateien und des lokalen Testservers. Insbesondere Klickabläufe, iPhone-Hoch-/Querformat, echte Hintergrund-Timerzeiten, Service-Worker-Offlinebetrieb und Import/Export im Browser wurden daher **nicht praktisch verifiziert**. Vor dem produktiven Einsatz auf dem iPhone bitte diese Punkte testen und vorher ein JSON-Backup erstellen.

## Update-Hinweis
Alle sieben Dateien im GitHub-Repository ersetzen, committen und die App nach der Pages-Bereitstellung neu öffnen. Bei älteren zwischengespeicherten Versionen kann ein weiterer Neustart der Web-App nötig sein.


## iPhone-Duo-Anpassung
Responsive CSS-Breakpoints fuer kompakte und aufgeklappte Ansichten, Querformat, Safe Areas und Modale ergaenzt. Ein echter Geraetetest auf iPhone Duo wurde nicht durchgefuehrt.


## Duo-Navigation zurückgesetzt
Die Navigation wurde auf eine feste untere Leiste zurückgesetzt. ZIP-Integrität und JavaScript-Syntax wurden geprüft. Ein echter iPhone-Gerätetest wurde nicht durchgeführt.


## Cinematic HUD Update – Prüfgrenzen
Zusätzliche Animationen sind CSS-basiert und greifen nicht in Projekt- oder Timerdaten ein. ZIP-Integrität und JavaScript-Syntax werden geprüft. Kein echter iPhone-Gerätetest und keine vollständige Browser-Regression durchgeführt.
