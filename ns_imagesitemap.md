# neusued Google Bilder-Sitemap

Das Plugin stellt unter /image-sitemap.xml eine eigene Sitemap mit Galeriebildern und lokalisierten Produkttiteln bereit.

Version 1.0.0 · JTL-Shop ab 5.3.0

## Installation

1. Das Plugin über die JTL-Pluginverwaltung installieren und aktivieren.
2. Die Adresse /image-sitemap.xml auf der eigenen Shop-Domain im Browser öffnen und die XML-Ausgabe prüfen.
3. Falls bereits ein anderes Plugin dieselbe Route /image-sitemap.xml bereitstellt, nur eines davon aktiv lassen.

## Konfiguration

1. Unter Plugins → neusued Google Bilder-Sitemap Bildgröße (lg oder xl), WebP-Ausgabe, Varianten und Cache-Dauer einstellen.
2. In der robots.txt sowohl die bestehende JTL-Sitemap als auch die Bilder-Sitemap eintragen.
3. Beide Sitemap-Adressen in der Google Search Console einreichen; den Cache bei Bedarf im Reiter „Status & URL“ leeren.

## Hinweise

- Die Bilder-Sitemap wird nicht automatisch in robots.txt eingetragen. Sobald Sie dort selbst eine Sitemap-Zeile ergänzen, müssen Sie auch die JTL-Standard-Sitemap ausdrücklich aufführen.

Support: https://help.neusued.de/support/
