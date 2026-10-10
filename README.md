# Dome DJ-Prüfapp – V2.3 Teststand

Aufbauend auf V2.2. Bestehende IndexedDB-Daten bleiben erhalten, sofern dieselbe GitHub-Pages-Adresse und derselbe Browser genutzt werden.

## Neu
- „Ausrede“ bei Reinigung und Getränkeresten anklickbar; Eingabe optional bei Ja und verpflichtend bei Nein (wie bisher die Begründung).
- Bei technischen Geräten optionale Bemerkung per Klick einblendbar; bei Defekt verpflichtend sichtbar.
- Archiv zeigt nur tatsächlich ausgefüllte Bemerkungen und Ausreden.
- Archivnavigation: Klick auf die obere Registerkarte „Kontrolle“ führt aus einem geöffneten archivierten Bogen zurück zum aktuellen Kontrollbogen/Arbeitsplatz.
- Veranstaltungstag bleibt vor Übernahme des Arbeitsplatzes über das Datumsfeld änderbar.
- Cache-Version erhöht, damit Änderungen nach Aktualisierung geladen werden.

## Noch offen
- Kontrollierte Arbeitsplatzkorrektur nach Übernahme ist noch nicht umgesetzt. Bitte noch nicht testen.
- Keine zentrale Synchronisierung zwischen Smartphones; alle Daten lokal im jeweiligen Browser.

## Installation
Dateien aus diesem ZIP **direkt ins Stammverzeichnis** des bestehenden GitHub-Pages-Repositories laden und vorhandene Dateien überschreiben. Keine Unterordner anlegen. Danach Seite neu laden (Strg+F5), gegebenenfalls nochmals öffnen, damit der neue Service Worker aktiv wird. Vorher zur Sicherheit im Menü „Einstellungen“ alle Bögen als JSON exportieren.
