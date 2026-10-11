# Dome DJ-Prüfapp – V2.3.4 Teststand

Aufbauend auf V2.3.3. Bestehende lokale IndexedDB-Kontrollbögen bleiben bei Aktualisierung derselben GitHub-Pages-Adresse und desselben Browsers erhalten. Keine automatische Synchronisierung zwischen Smartphones.

## Änderungen
- Archiv: Gesamtexport aller Bögen als JSON direkt in der Archivübersicht. Sicherungsimport weiterhin unter Einstellungen.
- Archiv: Soundcheck-Einträge und Bemerkungen zu Reinigung/Getränkeresten gut sichtbar; Archivgruppen „Mit Beanstandungen“ / „Ohne Beanstandungen“.
- Einzelbogen: Im Archiv auf „Lesen“ klicken, unten „Diesen Bogen als PDF speichern / drucken“ wählen. Im Browser-Druckdialog „Als PDF speichern“ auswählen. Dies ist kein direkter PDF-Download; Pop-ups müssen ggf. erlaubt werden.
- Soundcheck-Überschrift: „Schäden bereits beim Soundcheck festgestellt“.
- Admin: Geräte direkt einem anderen Standard-Setup zuordnen; bisherige Zuordnung wird beim Speichern automatisch aufgehoben.
- Admin: ein Feld „Gerätename (Gerätenummer)“, Kategorie als Pull-down. Interne IDs bleiben bestehen.
- Admin: Kategorien hinzufügen, umbenennen und entfernen, sofern keine Geräte mehr zugeordnet sind.
- Admin: breitere Darstellung auf Desktop-Bildschirmen.
- Reinigung: gemeinsames Textfeld „Ausreden / Beanstandungen“.

## Installation
Alle sieben Dateien aus dem ZIP direkt in das Stammverzeichnis des bisherigen GitHub-Pages-Repositories hochladen und vorhandene Dateien ersetzen. Vorher die lokalen Bögen unter Archiv als JSON sichern. Danach Seite aktualisieren, ggf. Strg+F5. **Nicht** Browser-Website-Daten löschen, da die Bögen lokal gespeichert werden.

## Grenzen
- Testversion ohne geschützten Admin-Zugang, ohne Nextcloud-Anbindung und ohne geräteübergreifende Synchronisierung.
- PDF wird über den Druckdialog erstellt, nicht automatisch im Hintergrund.
- DJ-seitige Auswahl eines Ersatzgeräts bleibt einer späteren Version vorbehalten.
- Bestehende offene Bögen übernehmen Setupänderungen weiterhin nur über „Setup aktualisieren“.
