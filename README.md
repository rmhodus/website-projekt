
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
├── Hotel
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

| Thema | Entscheidung | Grund |
|---|---|---|
| Technik | Reines HTML und CSS, kein JavaScript | Vorgabe |
| CSS | Eigenes CSS mit `@layer`, kein Framework | Kleine Dateien |
| Farben | Nur als Variablen in `tokens.css` | Einheitlich, an einer Stelle änderbar |
| Responsive | Mobile-first, breites Layout ab `64rem` | Lesbar von 320 bis 1920 px |
| Menü | `popover` auf dem Handy | Ohne JavaScript, mit Tastatur bedienbar |
| Formular | HTML-Validierung, sendet auf `danke.html` | Kein Backend |
| Bilder | WebP mit `width` und `height` | Schnelles Laden |


## Testhinweise

- Über einen lokalen Server öffnen, nicht per Doppelklick.
- Getestet in aktuellen Versionen von Chrome, Firefox und Safari.
- Breiten 320, 768, 1280, 1920 px (DevTools → Device Toolbar).
- Langsames Netz: DevTools → Network → *Slow 4G*.
- Alles ist mit der Tastatur bedienbar.
- Geprüft mit [W3C Validator](https://validator.w3.org/) und [accessibilitychecker.org](https://www.accessibilitychecker.org/).


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
| Fotos | Unsplash | Unsplash License |
| Schrift | Google Fonts, lokal gespeichert | SIL Open Font License |
