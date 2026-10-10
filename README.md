# Dome DJ-Prüfapp V2.1 – interner Teststand

Ausgehend von V2, mit unverändertem IndexedDB-Namen `dome-dj-check` und unveränderten Stores. Vor dem Update beide JSON-Exporte sichern.

## Änderungen
- Abschluss archiviert den Bogen sofort, sperrt ihn und kehrt zur Kontrolle zurück. Bei Defekten wird die E-Mail-Vorbereitung **freiwillig** angeboten; der tatsächliche Versand bleibt manuell.
- Mehrere Bögen am selben Datum/Arbeitsplatz sind lokal möglich (neue eindeutige Bogen-IDs). Vorhandene V1/V2-Bögen bleiben lesbar. Offene Bögen werden beim Aufruf weitergeführt.
- Lokales Archiv zeigt getrennte Gruppen „Mit Defekten“ / „Ohne Defekte“ (nur abgeschlossene Bögen). Diese Gruppierung bereitet die spätere Nextcloud-Ordnerstruktur vor, legt aber keine Nextcloud-Ordner an.
- Frühere Prüfungen entfernter Geräte werden unter „Setupänderungen während der Schicht“ sichtbar; bestehende V2-Änderungsvermerke werden angezeigt.
- Admin kann Gerätebezeichnung und Kategorie nachträglich bearbeiten. Die Gerätenummer bleibt in dieser Version unverändert, um bestehende Referenzen zu schützen.
- Ein Gerät kann nicht mehr über die Setup-Verwaltung gleichzeitig zwei Arbeitsplätzen zugeordnet werden.
- Service-Worker-Cache-Version aktualisiert.

## Grenzen und Sicherheit
- Weiterhin **nur interner Teststand**. Admin- und Archiv-Reiter sind öffentlich zugänglich, wenn die App über GitHub Pages veröffentlicht wird. Noch keine geschützte DJ-Oberfläche, kein Authentifizierungsdienst und keine Nextcloud-Anbindung. Keine realen personenbezogenen oder vertraulichen Betriebsdaten verwenden.
- Daten werden ausschließlich im jeweiligen Browser gespeichert; keine automatische Übertragung zwischen Geräten.
- Kein PDF-Export und keine serverseitige Archivierung.
- Der E-Mail-Empfänger wird lokal in Einstellungen gespeichert; eine E-Mail wird nur im Mailprogramm vorbereitet, nicht automatisch versendet.
- Konfigurationsexport bleibt im Format `dome-equipment-v2`, um mit bestehenden V2-Sicherungen kompatibel zu sein.

## Installation / Test
Dateien **direkt im GitHub-Repository-Hauptverzeichnis** hochladen (`index.html` muss im Root liegen), dann GitHub Pages über `main` / `(root)` bereitstellen. Vor dem Test beide JSON-Exporte sicher aufbewahren. Nach Aktualisierung ggf. Seite neu laden; die Offline-App aktualisiert sich über den Service Worker.
