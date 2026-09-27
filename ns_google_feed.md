# neusued Google Merchant Feed

Das Plugin überträgt Produkte per Google Merchant API v1 an das Merchant Center und bietet einen optionalen XML-Feed.

Version 2.2.0 · JTL-Shop ab 5.5.0

## Installation

1. Das Plugin über die JTL-Pluginverwaltung installieren und aktivieren.
2. Unter System → Cron einen Job vom Typ ns_gfeed_sync mit einem Intervall von etwa einer Stunde einrichten. Ohne diesen Job findet keine verlässliche Übertragung statt.
3. In Google Cloud die Merchant API aktivieren, einen Service-Account mit JSON-Schlüssel anlegen und dessen E-Mail im Merchant Center als Nutzer berechtigen.

## Konfiguration

1. Unter „Kanäle → Bearbeiten“ Merchant-ID und Service-Account-JSON hinterlegen, Sprache, Währung und Zielland prüfen und speichern.
2. „Verbindung testen“ ausführen; dabei wird die Merchant API tatsächlich kontaktiert.
3. In der Kanalliste „Jetzt synchronisieren“ oder „Alle Produkte synchronisieren“ wählen und anschließend Dashboard sowie „Analyse → Qualität & Ablehnungen“ prüfen.

## Hinweise

- Der JSON-Schlüssel ist vertraulich und gehört nur in das dafür vorgesehene Plugin-Feld.
- Die optionale KI-Optimierung ist standardmäßig deaktiviert.

Support: https://help.neusued.de/support/
