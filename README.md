# Dome DJ-Prüfapp V2.2 – interner Teststand

## Änderungen gegenüber V2.1
- Admin: Arbeitsplatz-Setup zuerst; Gerätekatalog darunter standardmäßig eingeklappt.
- Interne technische Gerätekennungen in den Bedienoberflächen ausgeblendet. Tatsächliche Gerätenummer separat bearbeitbar, auch leer möglich. Vorhandene `ALT-...`-Kennungen werden bei Übernahme nicht als echte Gerätenummer behandelt. Alte, manuell vergebene Kennungen bleiben als tatsächliche Nummer erhalten, bis sie geändert werden.
- Neue Geräte bekommen zufällige technische Kennungen im Hintergrund. Die technische Kennung vorhandener Geräte bleibt für die Zuordnungen erhalten.
- Gerätebemerkungen sind unabhängig vom Prüfstatus möglich; bei Defekten weiterhin Pflicht.
- Wechsel aus einer archivierten Leseansicht zurück zur Kontrolle setzt die Auswahl zurück; „Zur Arbeitsplatzwahl“ ebenfalls.
- Veranstaltungstag = Datum des Veranstaltungsbeginns; nach Mitternacht bei Bedarf manuell einstellen.
- Für einen weiteren Kontrollbogen am selben Arbeitsplatz/Veranstaltungstag wird beim Übernehmen gewarnt und eine verpflichtende Begründung abgefragt. Die Begründung erscheint im Kontrollbogen und im Archiv.
- JSON-Import akzeptiert auch die eindeutigen V2.1-Bogen-IDs. Vorhandene Datensätze werden beim Import nicht überschrieben.
- Neuer Offline-Cache-Name.

## Grenzen
Nur lokaler Teststand auf GitHub Pages: Admin-Bereich und Archiv **nicht zugriffsgeschützt**. Keine zentrale Synchronisation, keine Nextcloud-Anbindung und kein PDF-Export. Keine echten sensiblen Daten auf öffentlich zugänglichen Testgeräten verwenden. Warnung zu bereits vorhandenem Bogen prüft **nur den lokalen Browser**, nicht andere Smartphones.

## Upgrade
Beide JSON-Exporte vorher sichern. Dateien im Root des bestehenden Testrepositorys ersetzen. IndexedDB-Name und Stores bleiben gleich. Bestehende archivierte Bögen bleiben unverändert; historische Anzeigen können noch frühere Gerätebezeichnungen enthalten. V2.2 ist noch nicht im Browser getestet.
