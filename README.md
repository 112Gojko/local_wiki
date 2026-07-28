# Praktikums-Wiki

Statisches HTML-Wiki zur Dokumentation eines Praktikums (Zeitraum ab 06.07.2026), navigierbar
nach Tagen und nach Projekten, mit Quellenangabe zu jeder Aussage. Dient als Grundlage für die
Präsentation gegenüber Praktikumsbetreuer und Schule.

## Struktur

```
Local_Wiki/
├── README.md
├── index.html              Startseite
├── assets/
│   └── style.css           gemeinsames Stylesheet für alle Seiten
├── nach-tagen/
│   ├── index.html           Übersicht, gruppiert nach Woche
│   ├── _vorlage.html        Kopiervorlage für eine neue Tagesseite
│   └── JJJJ-MM-TT.html       eine Seite pro Tag (Dateiname = ISO-Datum)
└── nach-projekten/
    ├── index.html           Übersicht aller Projekte
    ├── _vorlage.html        Kopiervorlage für eine neue Projektseite
    └── [projektname].html   eine Seite pro Projekt
```

## Navigationsprinzip

- **`nach-tagen/`** ist eine kurze, chronologische Linkliste pro Tag.
- **`nach-projekten/`** enthält den eigentlichen, ausführlichen Text pro Projekt.
- Tagesseiten verlinken auf die zugehörige Projektseite, statt den Text zu duplizieren.

## Quellenangaben

Jede Aussage bekommt einen Quellenlink, unterschieden nach Art:

- `quelle--intern` – Verweis auf eigene Projektdateien/Commits/Tickets
- `quelle--extern` – Verweis auf externe Doku/Tools/Tutorials

Siehe `nach-projekten/_vorlage.html` für die Markup-Beispiele.

## Zuordnung Tag → Projekt

Die Zuordnung, welcher Tag zu welchem Projekt gehört, steht in
`Praktikum_Mit_Datum.xlsx` (Spalten "Zuordnung Wiki (Haupt)" / "(Neben)").

<!-- TODO: eigener Abschnitt, z.B. Lieblingsprojekt / Fazit, falls gewünscht. -->
