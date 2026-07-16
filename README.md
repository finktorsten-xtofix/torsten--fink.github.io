# torsten-fink.de — Reisen, Fotografie & Geschichten

**Live:** [https://torsten-fink.de](https://torsten-fink.de)

Persönliche Website von **Torsten Fink** — Reiseerzähler, Fotograf und Golfer aus Fürth.
Sieben Reisegeschichten zwischen Tokio und Bad Heilbrunn, erzählt in eigenem Ton und bebildert mit eigenen Fotografien.

## Geschichten

| Jahr | Geschichte |
|---|---|
| 2026 | [Bad Heilbrunn — Bayerisches Lakeland](https://torsten-fink.de/stories/bad-heilbrunn.html) |
| 2026 | [Beldibi — Türkisfarbenes Wasser & Russische Geschichten](https://torsten-fink.de/stories/beldibi.html) |
| 2025 | [Locarno & Ascona — Das Tessin im Entschleunigungsmodus](https://torsten-fink.de/stories/ascona.html) |
| 2023 | [Istanbul — Das Tor Asiens](https://torsten-fink.de/stories/istanbul.html) |
| 2019 | [Hongkong — Ein Duft von Abenteuer und Feuerwerk](https://torsten-fink.de/stories/hongkong.html) |
| 2017 | [Tokio — Der Puls einer Welt, die niemals schläft](https://torsten-fink.de/stories/tokio.html) |
| 2015 | [Singapur — Eine Stadt, die man nicht besucht, sondern absolviert](https://torsten-fink.de/stories/singapur.html) |

## Technik

- **Hosting:** GitHub Pages, Custom Domain `torsten-fink.de` (CNAME-Datei im Root — nicht löschen!), HTTPS erzwungen
- **Stack:** Pures HTML/CSS, kein Framework, kein Build-Prozess, keine Cookies, kein Tracking
- **Design:** Dunkles Kino-Theme, EXIF-Daten als Gestaltungselement, japanische Typografie, Filmstreifen-Galerie
- **Schriften:** Syne · Instrument Sans · IBM Plex Mono · Noto Serif JP (Google Fonts)
- **SEO/KI:** JSON-LD (Person, WebSite, Blog + BlogPostings), `sitemap.xml`, `robots.txt`, `llms.txt`, Open Graph, Twitter Cards

## Struktur

```
├── index.html            Startseite
├── stories/              Sieben Reisegeschichten
├── assets/
│   ├── css/story.css     Stylesheet der Unterseiten
│   └── images/           Optimierte Fotos (Startseite + stories/)
├── impressum.html        § 5 DDG
├── datenschutz.html      DSGVO
├── sitemap.xml · robots.txt · llms.txt · 404.html · CNAME
```

## Pflegehinweise (Notizen an mich selbst)

1. **Bilder vor dem Upload optimieren:** max. 1600 px, JPEG-Qualität ~82, Ziel < 600 KB. Keine Umlaute oder Leerzeichen in Dateinamen.
2. **Ordner beachten:** Story-Bilder nach `assets/images/stories/`, Story-Seiten nach `stories/` — beim GitHub-Upload immer erst **in den Zielordner navigieren**, dann hochladen.
3. **Neue Geschichte = fünf Baustellen:** Story-HTML, Eintrag in `index.html` (Liste + JSON-LD + ggf. Galerie), `sitemap.xml`, `llms.txt`, Pager-Links der Nachbar-Stories.
4. **CNAME-Datei** und Custom-Domain-Einstellung nicht anfassen — sonst startet die Zertifikats-Ausstellung neu.
5. Nach jedem Inhalts-Update: neue URL in der Google Search Console zur Indexierung einreichen.

## Rechtliches

Alle Fotografien und Texte © Torsten Fink. Alle Rechte vorbehalten — keine Nutzung ohne schriftliche Zustimmung.
Der Code (HTML/CSS) darf gern als Inspiration dienen.

---

*Die nächste Geschichte lädt schon hoch.* 📷
