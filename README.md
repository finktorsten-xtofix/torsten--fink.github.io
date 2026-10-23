# torsten-fink.de — Reisen, Fotografie & Geschichten

**Live:** [https://torsten-fink.de](https://torsten-fink.de)

Persönliche Website von **Torsten Fink** — Reiseerzähler, Fotograf und Golfer aus Fürth.
Neun Reisegeschichten zwischen Kamakura und Bad Heilbrunn, dazu eine Golf-Story vom Heimatclub, erzählt in eigenem Ton und bebildert mit eigenen Fotografien.

## Geschichten

| Jahr | Geschichte |
|---|---|
| 2026 | [Passau — Drei Flüsse verbinden Lebenslust und Kultur](https://torsten-fink.de/stories/passau.html) |
| 2026 | [Bad Heilbrunn — Bayerisches Lakeland](https://torsten-fink.de/stories/bad-heilbrunn.html) |
| 2026 | [Beldibi — Türkisfarbenes Wasser & Russische Geschichten](https://torsten-fink.de/stories/beldibi.html) |
| 2025 | [Locarno & Ascona — Das Tessin im Entschleunigungsmodus](https://torsten-fink.de/stories/ascona.html) |
| 2023 | [Istanbul — Das Tor Asiens](https://torsten-fink.de/stories/istanbul.html) |
| 2019 | [Hongkong — Ein Duft von Abenteuer und Feuerwerk](https://torsten-fink.de/stories/hongkong.html) |
| 2017 | [Kamakura — Wo die Shogun surften?](https://torsten-fink.de/stories/kamakura.html) |
| 2017 | [Tokio — Der Puls einer Welt, die niemals schläft](https://torsten-fink.de/stories/tokio.html) |
| 2015 | [Singapur — Einmal hoch und runter im SG50-Jahr](https://torsten-fink.de/stories/singapur.html) |

## Golf

| Story | Beschreibung |
|---|---|
| [Golf Club Herzogenaurach — Golf spielen, weil es Spaß macht](https://torsten-fink.de/stories/herzogenaurach.html) | Heimatclub, Craig Miller Golfschule, die Adidas/Puma-Geschichte der Stadt. Von der Startseite aus über den Golf-Bereich verlinkt, läuft nicht in der Pager-Reihenfolge der neun Reisegeschichten mit. |

## Reise-Wissen

| Seite | Beschreibung |
|---|---|
| [Tokio zu Fuß: 8 Bahnhöfe](https://torsten-fink.de/guides/tokio-bahnhoefe-zu-fuss.html) | Acht Tokioter Bahnhöfe mit Gehzeiten aus offiziellen Quellen, schematischer Karte (Bild im Ring: KI-Fotomontage, gekennzeichnet) und eigenen Fotos. Schema Article + BreadcrumbList. Läuft außerhalb der Pager-Reihenfolge. |
| [Verbeugen in Japan](https://torsten-fink.de/guides/japan-verbeugung-ojigi.html) | Eshaku, Keirei, Saikeirei, Dogeza mit Winkeln, Anlässen und Beispielsätzen. Grafik selbst gesetzt, Figuren sind Fotos von Torsten (keine KI). |
| [Tai Chi in Hongkong](https://torsten-fink.de/guides/hongkong-tai-chi.html) | Herkunft, belegte Wirkung und eine Beispielübung in vier Phasen. Grafik selbst gezeichnet (keine KI), Fotos von Torsten (Aberdeen 2015, Central 2019, mit Erlaubnis). |

## Tools

| Tool | Beschreibung |
|---|---|
| [Handicap-Rechner](https://torsten-fink.de/tools/handicap-rechner.html) | Score Differential, Handicap-Index und Course Handicap nach WHS inkl. 9-Loch-Runden, PCC, außergewöhnlichen Runden, Soft/Hard Cap und 26,5-Bremse, Rechenweg zum Aufklappen. Reines Vanilla-JS, Speicherung nur im `localStorage` des Browsers, Export/Import als JSON, keine Anmeldung, kein Server-Backend. |
| [Stableford-Rechner](https://torsten-fink.de/tools/stableford-rechner.html) | Playing Handicap nach WHS mit Vorgabe-Prozentsatz, Vorgabeschläge pro Loch nach Stroke Index inkl. Plus-Handicaps, Netto- und Bruttopunkte für 18 oder 9 Löcher, Rechenweg zum Aufklappen. Speichert laufende Runde und gemerkte Plätze im `localStorage`, übernimmt den Index aus dem Handicap-Rechner (`golf:hi`). Plätze lassen sich per Link teilen (Daten im URL-Hash, Umami mit `data-exclude-hash`). |
| [Jetlag-Rechner](https://torsten-fink.de/tools/jetlag-rechner.html) | Zeitzonen-Unterschied inkl. Sommer-/Winterzeit berechnen, Tag-für-Tag-Anpassungsplan. Verlinkt aus Tokio, Kamakura, Hongkong und Singapur. Reines Vanilla-JS, keine Anmeldung, kein Server-Backend. |

## Technik

- **Hosting:** GitHub Pages, Custom Domain `torsten-fink.de` (CNAME-Datei im Root — nicht löschen!), HTTPS erzwungen
- **Stack:** Pures HTML/CSS, kein Framework, kein Build-Prozess, keine Cookies
- **Reichweitenmessung:** Umami Cloud, cookielos, auf allen Seiten eingebunden. Handicap-Rechner und Stableford-Rechner speichern Eingaben nur im `localStorage` des Browsers. Details in `datenschutz.html`, Abschnitte 5 und 6.
- **Design:** Dunkles Kino-Theme, EXIF-Daten als Gestaltungselement, japanische Typografie, Filmstreifen-Galerie
- **Schriften:** Syne · Instrument Sans · IBM Plex Mono · Noto Serif JP (Google Fonts)
- **IndexNow:** GitHub-Aktion `.github/workflows/indexnow.yml` meldet nach jedem Push auf `main` neue oder geänderte HTML-Seiten an Bing und die übrigen IndexNow-Suchmaschinen (nicht Google). Von Hand unter Actions → IndexNow → Run workflow: alle Seiten aus `sitemap.xml`. Schlüsseldatei `705f3334de5bd9d14abfc21e1fd270c6.txt` im Root nicht löschen.
- **SEO/KI:** JSON-LD (Person, WebSite, Blog + BlogPostings), `sitemap.xml`, `robots.txt`, `llms.txt`, Open Graph, Twitter Cards, Quellenverzeichnis am Ende jeder Story (Kicker „Quellen & Recherche", verlinkte Quellenliste als GEO-Signal)

## Struktur

```
├── index.html            Startseite
├── stories/              Neun Reisegeschichten + eine Golf-Story (Herzogenaurach)
├── guides/               Reise-Wissen: Tokio zu Fuß, Verbeugen in Japan, Tai Chi in Hongkong
├── tools/                Interaktive Tools: Handicap-Rechner, Stableford-Rechner, Jetlag-Rechner
├── assets/
│   ├── css/story.css     Stylesheet der Unterseiten
│   └── images/           Optimierte Fotos (Startseite, stories/, guides/, tools/)
├── impressum.html        § 5 DDG
├── datenschutz.html      DSGVO
├── sitemap.xml · robots.txt · llms.txt · 404.html · CNAME
```

## Rechtliches

Alle Fotografien und Texte © Torsten Fink. Alle Rechte vorbehalten — keine Nutzung ohne schriftliche Zustimmung.
Der Code (HTML/CSS) darf gern als Inspiration dienen.

---

*Die nächste Geschichte lädt schon hoch.* 📷
