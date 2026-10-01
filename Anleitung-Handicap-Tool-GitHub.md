# Anleitung: Handicap-Rechner in GitHub pflegen

Stand: 30.09.2026, Version 2 des Rechners (WHS mit 9-Loch-Runden, PCC und Rechenweg).

Der Ordner `tools/` existiert bereits, der Rechner ist live verlinkt. Eine Ersteinrichtung ist nicht mehr nötig. Diese Anleitung beschreibt das Aktualisieren.

## 1. Stand im Repo (geprüft am 01.10.2026, alles aktuell)

| Datei | Ziel im Repo | Status |
|---|---|---|
| `handicap-rechner.html` | `tools/` | Version 2 ist live. GBE statt Brutto, 9-Loch-Runden, PCC, außergewöhnliche Runden, Soft/Hard Cap, 26,5-Bremse, Rechenweg, Plätze merken, Export/Import, Quellenabschnitt |
| `sitemap.xml` | Root | Aktuell, `lastmod` des Rechners 2026-09-30 |
| `llms.txt` | Root | Aktuell, Beschreibung des Rechners auf Version 2 |
| `README.md` | Root | Aktuell, Tools-Tabelle und Zeile zur Reichweitenmessung |
| `datenschutz.html` | Root | Aktuell, Abschnitt 6 zur lokalen Speicherung des Rechners |
| `Anleitung-Handicap-Tool-GitHub.md` | Root | Diese Datei |

`index.html` bleibt unverändert, der Button „Golf-Handicap-Rechner öffnen“ zeigt weiterhin auf `tools/handicap-rechner.html`. Die Pager-Verlinkung aus `stories/herzogenaurach.html` bleibt ebenfalls gültig.

## 2. Hochladen bei künftigen Updates

Im Repository erst in den Zielordner navigieren (`tools/` für den Rechner, Root für `sitemap.xml`, `llms.txt`, `README.md`, `datenschutz.html`), dann **Add file → Upload files**. GitHub ersetzt vorhandene Dateien mit gleichem Namen. Die Reihenfolge ist egal, solange keine neue URL entsteht.

## 3. Kontrolle nach dem Upload

GitHub Pages braucht nach dem Commit meist ein bis zwei Minuten. Danach:

- `https://torsten-fink.de/tools/handicap-rechner.html` aufrufen, bei Bedarf mit Strg+F5 neu laden
- **Alte Runden:** Wer mit Version 1 schon Runden gespeichert hat, sieht sie weiterhin. Der alte Wert „Score“ wird als GBE übernommen, alle Runden gelten als 18-Loch-Runden mit PCC 0.
- **18-Loch-Test:** GBE 91, CR 71,2, Slope 128, PCC +1 ergibt das Differential 16,6
- **9-Loch-Test:** Unter Einstellungen einen Club-Index eintragen, z. B. 14,0. Dann eine 9-Loch-Runde mit GBE 41, CR 34,6, Slope 100 erfassen. Erwartet wird das Differential 15,7, das Beispielergebnis aus dem USGA-Infoblatt zu 9-Loch-Runden.
- **Speichern:** Seite neu laden, die Runden müssen noch da sein
- **Handy:** Seite auf dem Smartphone öffnen, nichts darf seitlich überstehen
- **Testdaten entfernen:** Einstellungen → „Alle Daten löschen“

## 4. Search Console

Nach dem Update die URL `https://torsten-fink.de/tools/handicap-rechner.html` in der Google Search Console über die URL-Prüfung erneut zur Indexierung einreichen. Titel und Description haben sich geändert.

## 5. Weitere Tools

Ein neues Tool kommt als weitere Datei in den Ordner `tools/`. Dazu jeweils ein Eintrag in `index.html`, `sitemap.xml`, `llms.txt` und in der Tools-Tabelle von `README.md`. Der Jetlag-Rechner ist nach diesem Muster eingebunden.

## Unterschied zu „neue Story hinzufügen“

Eine neue Story umfasst laut `README.md` (Pflegehinweise) sechs Baustellen, darunter das Quellenverzeichnis und die Pager-Links der Nachbar-Storys. Ein Tool läuft nicht in der Pager-Kette mit und hat keine Galerie-Einbindung. Deshalb reichen fünf Baustellen: Tool-HTML, `index.html`, `sitemap.xml`, `llms.txt`, `README.md`.

## Geplante Erweiterung: Platzdatenbank

Noch nicht umgesetzt. Idee: eine Datei `tools/plaetze.json` mit Club, Schleife, Abschlag, CR, Slope, Par, Stand und Quelle je Eintrag. Sie wird Platz für Platz aus den Angaben der Clubs aufgebaut, nicht aus fremden Datenbanken übernommen (Datenbankschutz nach § 87b UrhG).
