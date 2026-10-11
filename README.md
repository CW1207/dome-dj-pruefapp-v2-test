# Dome DJ-Prüfapp – V2.3.5 Teststand

Aufbauend auf V2.3.4. Die lokale IndexedDB-Datenbank wird nicht gelöscht oder migriert.

## Änderungen
- Smartphone-Ansichten DJ und Technik/Admin. DJ blendet Archiv, Einstellungen und Admin aus; Technik/Admin bietet alle Bereiche. **Nur UI-Trennung, noch keine Zugriffssperre.**
- Archiv: Einträge standardmäßig geschlossen, Kopfzeile mit Datum · Bereich · DJ. Aufklappen zeigt den gesamten archivierten Bogen direkt, einschließlich PDF- und ggf. E-Mail-Funktion; kein Lesen-Button.
- Drucklayout: A4, Gerätezeilen sollen nicht mitten im Eintrag getrennt werden; längere Inhalte können mehrere Seiten belegen.
- Admin: Zuordnungen werden sofort beim Anhaken gespeichert; Geräte werden aus anderen Bereichen entfernt.
- Überschriften: „Kontrolle des Setup und Technik“ und „Beanstandungen Soundcheck“.
- Keine breitere Desktop-Sonderansicht.

## Installation und Test
Alle sieben Dateien aus dem ZIP ins Stammverzeichnis des bisherigen GitHub-Pages-Repositories hochladen und die bisherigen ersetzen. **Vorher das Archiv als JSON sichern.** Nach der Veröffentlichung Seite neu laden, ggf. Strg+F5. Niemals Website-Daten löschen: Darin liegen die lokalen Bögen.

## Grenzen
- Beide Ansichten nutzen dieselbe lokale Datenbasis, keine Synchronisierung zwischen Geräten.
- Die Technik/Admin-Ansicht ist nicht gegen unbefugte Nutzung geschützt.
- PDF-Export über den Browserdruckdialog; Nextcloud-PDF-Ablage ist weiterhin geplant, aber noch nicht umgesetzt.
- Das spätere getrennte Standard-Referenzsetup samt Reset sowie die Veranstaltungslogistik sind nicht Teil dieser Version.
