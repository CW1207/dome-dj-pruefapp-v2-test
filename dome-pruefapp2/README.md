# Dome DJ-Prüfapp – Version 2 (lokaler Entwicklungsstand)

Diese Version baut auf dem Originalprototyp auf und behält die IndexedDB `dome-dj-check` sowie die vorhandenen Kontrollbögen bei.

## Neu
- Bestätigte Bereichsübernahme pro Kontrollbogen; Wechsel von Bereich/Datum danach gesperrt.
- Abgeschlossene Kontrollbögen im normalen App-Ablauf dauerhaft schreibgeschützt.
- Lokaler Equipment-Katalog mit eindeutigen Gerätenummern und Zuordnung zu Main Stage, Main FOH, Stadl und La Vie.
- Main FOH standardmäßig im DJ-Auswahlmenü deaktiviert, aber im Admin-Testbereich aktivierbar.
- Manuelle Setup-Aktualisierung offener Bögen; Ergebnisse unveränderter Geräte bleiben erhalten.
- Import/Export von Equipment-Konfigurationen als JSON.
- Weiterhin offlinefähig mit lokaler Speicherung.

## Grenzen dieses Teststands
- **Keine Nextcloud-Anbindung**; Admin-Änderungen sind nur auf dem aktuellen Gerät sichtbar, außer bei manuellem Konfigurationsimport.
- **Kein echter Admin-Zugriffsschutz**. Der Admin-Reiter ist ausdrücklich nur für Tests gedacht, nicht für den produktiven Einsatz durch DJs.
- Geräte aus dem ursprünglichen Prototyp wurden mangels echter Inventarnummern mit vorläufigen Kennungen `ALT-001` usw. angelegt. Diese vor der Nutzung durch echte Nummern ersetzen.
- Bestehende V1-Bögen bleiben in ihrem bisherigen Format; die Sperre wird anhand des Abschlusszeitpunkts angewandt.
- Keine PDF-Erstellung und kein zentraler Upload; JSON-Sicherung bleibt vorhanden.
- Keine zuverlässige Identitätsprüfung und kein geräteübergreifender Schutz gegen Doppelbelegung.

## Testhinweise
App über HTTPS oder localhost ausliefern, nicht direkt über `file://` starten. Vor dem Test mit vorhandenen Daten eine JSON-Sicherung der V1 anlegen. Nach dem Update zuerst vorhandene Archivbögen und die Offlinefunktion prüfen. Ein abgeschlossener Bogen lässt sich im normalen UI nicht bearbeiten.
