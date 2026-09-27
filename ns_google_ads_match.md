# neusued Google Ads Kundenabgleich

Das Plugin überträgt einwilligungsberechtigte Käuferdaten als Hashes an eine Google Ads Customer-Match-Zielgruppe.

Version 1.6.0 · JTL-Shop ab 5.3.0

## Installation

1. Das Plugin über die JTL-Pluginverwaltung installieren und aktivieren.
2. In einem Google-Cloud-Projekt die Data Manager API aktivieren und Service-Account oder OAuth-Zugang vorbereiten.
3. Die verwendete Identität in Google Ads berechtigen und eine Customer-Match-Zielgruppe mit Zielgruppen-ID anlegen.

## Konfiguration

1. Im Plugin unter „Einstellungen“ Google-Ads-Konto-ID, gegebenenfalls MCC-ID, Zielgruppen-ID und Einwilligungs-Regel eintragen; Nutzungsbedingungen bestätigen.
2. Unter „Verbindung“ die Zugangsdaten hinterlegen und „Verbindung testen“ ausführen. Der Test nutzt validateOnly und speichert keine Zielgruppenmitglieder.
3. Erst nach erfolgreichem Test „Synchronisierung aktiv“ einschalten. Den automatisch angelegten Cronjob ns_gads_sync und den Status-Reiter prüfen.

## Hinweise

- Standard ist die ausdrückliche JTL-Consent-Manager-Einwilligung „Google Ads Kundenabgleich“. Newsletter-Einwilligung allein deckt eine Google-Datenweitergabe nicht automatisch ab.
- Unter der empfohlenen Consent-Regel übernimmt ein Backfill keine alten Kundendaten ohne nachweisbare Einwilligung.

Support: https://help.neusued.de/support/
