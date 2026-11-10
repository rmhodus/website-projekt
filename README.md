
# Fellness Hotel

Website des fiktiven Wellness Hotels "Fellness". Gestresste Berufstätige sollen hier eine Auszeit von ihrem Alltag nehmen können und entspannte Wellness-Zeit genießen können

> Fiktive Arbeit im Rahmen des Webseiten-Projekts an der DHBW Heidenheim. Das Wellness Hotel ist erfunden.


## Team

| Person | Aufgabe |
|---|---|
| Roman  | Technik |
| Florian | Technik |
| Max | Design |
| Till | Dokumentation |


## Ansehen

Nur HTML und CSS, keine Installation, kein JavaScript.

1. Repository klonen.
2. Im Projektordner einen lokalen Server starten:
   ```bash
   python3 -m http.server 8000
   ```
3. Im Browser `http://localhost:8000` öffnen. Einstieg ist `index.html`.


## Struktur

```
Startseite
├── Zimmer
│   └── Zimmer-Detail
├── Wellness
│   └── Wellness-Detail
├── Rezensionen
├── Über uns
├── Buchung
│   └── Danke
└── Impressum   (im Footer)

```


## Technische Grundlagen und Entscheidungen

| Thema | Entscheidung | Erläuterung |
|---|---|---|
| Technik | Reines HTML und CSS, kein JavaScript | Vorgabe |
| CSS | Eigenes CSS ohne Framework | in einer Datei css/stlye.css |
| Farben | Nur als Variablen in :root | Einheitlich, an einer Stelle änderbar |
| Responsive | Mobile-first, Breakpoints bei 48em (Tablet) und 64 em (Desktop) | Lesbar von 320 bis 1920 px |
| Menü | Auf dem Handy per Checkbox und Label ein- und ausklappbar, ab 64em immer sichtbar | Ohne JavaScript |
| Darkmode | Schalter per Checkbox und :checked, ohne Java Skript | Auswahl gilt nur auf der aktuellen Seite |
| Formular | HTML-Validierung, sendet auf `danke.html` | Kein Backend |
| Bilder | WebP mit `width` und `height` | Schnelles Laden |


## Testhinweise

- Über einen lokalen Server öffnen, nicht per Doppelklick.
- Gepalnt: Test in aktuellen Versionen von Chrome, Firefox und Safari.
- Breiten 320, 768, 1280, 1920 px (DevTools → Device Toolbar).
- Langsames Netz: DevTools → Network → *Slow 4G*.
- Alles soll mit der Tastatur bedienbar sein.
- Geplant: Prüfung mit [W3C Validator](https://validator.w3.org/) und [accessibilitychecker.org](https://www.accessibilitychecker.org/).


## Zusammenarbeit

1. Niemand committet direkt auf `main`.
2. Jede Aufgabe bekommt einen eigenen Branch vom aktuellen `main`.
3. Jeder Branch kommt über einen Pull Request nach `main`.
4. Eine andere Person prüft den Pull Request und gibt ihn frei. Wer den Pull Request geöffnet hat, mergt ihn.
5. Wer den Pull Request gemergt hat, löscht den Branch. Alle aktualisieren `main` mit `git pull`.

Commit-Nachrichten und Titel von Pull Requests folgen [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).


## Quellen und Lizenzen

| Inhalt | Quelle | Lizenz |
|---|---|---|
| Fotos | KI-generiert mit Google Gemini (eigene Promts nach unserem Konzept) | Nutzung gemäß Nutzungsbedingungen von Google Gemini |
| Schrift | Georgia und Systemschrift des Geräts, keine Webfonts | Systemschrift, mit dem Betriebssystem mitgeliefert |
