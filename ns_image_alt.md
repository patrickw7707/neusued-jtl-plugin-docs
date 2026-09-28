# neusued KI Bild-Alt-Texte

Bildbasierte Alt-Text-Vorschläge für eigene Produkt- und Galeriebilder. Nur ausdrücklich freigegebene Texte erscheinen im Shop.

Version 1.0.1 · JTL-Shop ab 5.7.1

## Voraussetzungen

- JTL-Shop ab 5.7.1; PHP gemäß den Anforderungen der eingesetzten Shop-Version (für 5.7.1 PHP 8.3+).
- PHP-Erweiterungen cURL, OpenSSL, mbstring sowie GD mit JPEG-, PNG- und WebP-Unterstützung.
- Eigener OpenRouter-API-Schlüssel, verfügbares Guthaben beziehungsweise Abrechnung und ein kompatibler Vision-Anbieter. Externe API-Kosten sind im Pluginpreis nicht enthalten.
- Eigene Produkt- und Galeriebilder in JPEG, PNG oder WebP aus dem Shop-Bildspeicher; höchstens 12 MiB und 24 Megapixel je Bild.
- Berechtigter Shop-Administrator für Bearbeitung und ausdrückliche Freigabe; Prüfung im eigenen Theme und in den verwendeten Sprachen.

## Installation

1. Im Shop-Backend Plugins → Meine Käufe öffnen, „Lizenzen erneut prüfen“ wählen und das Plugin über „Installieren“ installieren. Anschließend aktivieren. Alternativ das bereitgestellte Plugin-ZIP im Pluginmanager hochladen, installieren und aktivieren.
2. Den Reiter „Bild-Alt-Texte“ öffnen. Die Einrichtung zuerst im Testshop durchführen.
3. Nach einer Freigabe die tatsächliche Ausgabe in Produktgalerie und Produktlisten für jede verwendete Sprache und das eigene Theme prüfen.

## Konfiguration und Freigabe

1. Unter „OpenRouter-Einstellungen und Datenschutz“ den eigenen API-Schlüssel und ein kompatibles Vision-Modell mit strukturierten Ausgaben hinterlegen. Voreinstellung: openai/gpt-4.1-mini.
2. Datenschutzanforderungen und Anbietervereinbarungen prüfen, die Übertragung ausdrücklich bestätigen und Cloud-Generierung aktivieren. Sie ist zunächst ausgeschaltet.
3. Das Tageslimit einstellen: standardmäßig 50, maximal 500 versuchte Anfragen. Ein Limit ist keine Kostenobergrenze; OpenRouter rechnet separat ab.
4. Sprache, Produktname und Status wählen. „Vorschlag generieren“ erstellt einen Entwurf. Optional bis zu fünf neue Bilder der aktuellen Seite nacheinander verarbeiten; vorhandene Entwürfe und Freigaben werden übersprungen.
5. Bild und Text vergleichen, Sprache und sachliche Richtigkeit prüfen, den Entwurf bei Bedarf bearbeiten. „Entwurf speichern“ veröffentlicht ihn noch nicht.
6. Erst „Speichern und freigeben“ übernimmt den Text in die Shop-Ausgabe. „Freigabe widerrufen“ stellt die ursprüngliche Beschreibung wieder her. Eine neue Generierung oder Entwurfsänderung ersetzt eine bestehende Freigabe nicht.

## Hinweise

- OpenRouter und der gewählte Modellanbieter sind externe Dienste. Übertragen werden das verkleinerte Bild, Produktname, Sprache und Generierungsanweisung. Prüfen Sie personenbezogene oder vertrauliche Inhalte vorab.
- Ein leeres Schlüsselfeld behält den gespeicherten Schlüssel. „Gespeicherten Schlüssel löschen“ entfernt ihn. Nach einer Änderung des Shop-Schlüssels muss der API-Schlüssel neu hinterlegt werden.
- Fehlgeschlagene Antworten können trotzdem Anbietergebühren verursachen. Das Tageslimit zählt versuchte Anfragen. Es gibt keine automatischen Wiederholungen oder Cronjobs.
- Alt-Texte enthalten 3–180 Zeichen ohne HTML. Beschreiben Sie sichtbare Merkmale, verwenden Sie natürliche Begriffe und setzen Sie wichtige Informationen zuerst. Keine erfundenen Eigenschaften oder Werbeversprechen.
- Eigene Wawi-Daten und Core-Dateien werden nicht geändert. Freigabe widerrufen oder Plugin deaktivieren stellt die ursprüngliche Beschreibung wieder her. Bei Deinstallation mit Datenlöschung werden nur die eigenen Plugin-Daten entfernt.
- Artikel mit Kundengruppen-Sichtbarkeitseinschränkungen, verlinkte Bilder über artikelbildlink und Platzhalter ohne eigenen Katalogbild-Eintrag sind ausgeschlossen.
- Prüfen Sie die Ausgabe in Ihrem Theme. NOVA kann Listenbeschreibungen kürzen. Dekorative Bilder, Linkbezeichnungen und ausführliche Diagrammerklärungen gehören zur gesonderten Theme- und Inhaltsprüfung.
- Keine Garantie für Rankings, Indexierung, BFSG- oder DSGVO-Konformität. Die bezahlte externe OpenRouter-End-to-End-Abnahme und die Qualität realer Modellantworten sind für diesen Stand noch nicht nachgewiesen.

## Änderungen in 1.0.1

- Formulierungsvorgaben für natürliche Produktidentität, sichtbare Details und tatsächliche Galerieansichten präzisiert.
- Redaktionelle Prüfhilfe im Backend und Alt-Text-Leitfaden ergänzt.
- 180 Zeichen als technische Obergrenze erläutert; keine Keywordlisten, erfundenen Eigenschaften oder Ranking-Zusagen.

Support: https://help.neusued.de/support/
