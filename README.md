# Training Chart

Training Chart ist eine kleine Web-App, die Trainingsdaten aus einer CSV-Datei einliest und als interaktives Linien-Diagramm darstellt.

## Was das Projekt macht

- Visualisiert Gewichte (`lbs`) pro Trainingsgerät über die Zeit.
- Zeigt pro Datenpunkt optional die Dauer (`sec`) im Tooltip.
- Berechnet zusätzlich eine Durchschnittslinie (`Durchschnitt`) über alle vorhandenen Geräte pro Tag.
- Kann Geräte auf Wunsch alphabetisch/gruppiert darstellen (Schalter `Geräte gruppieren`).

## Schnellstart

1. Projektordner lokal öffnen.
2. Die Datei `index.html` im Browser starten (Doppelklick reicht).
3. Oben im Bereich **Datei auswählen** eine CSV-Datei laden (z. B. `training.csv`).
4. Optional den Schalter **Geräte gruppieren** aktivieren, um die Reihenfolge im Chart umzuschalten.

Die App ist außerdem öffentlich über GitHub Pages erreichbar:
[https://joergsteinhauer.github.io/trainingchart/](https://joergsteinhauer.github.io/trainingchart/)

## CSV-Format (Kurz)

- Trennzeichen: `;`
- Erste Spalte: Datum im Format `DD.MM.YYYY`
- Danach pro Gerät jeweils Gewicht und direkt dahinter Dauer:
  - Beispielkopf: `Datum;A3;;B7;;B1;`
  - Beispielwert: `01.01.2025;60,0 lb;90 s;110,0 lb;120 s;...`

Hinweis: Leere Felder werden ignoriert, unvollständige Zeilen sind also möglich.

## TODOs / Verbesserungen

Die bisherige Aufgabenliste wurde ausgelagert nach [`TODO.md`](TODO.md).

## Best Practices

- Keine sensiblen oder personenbezogenen Daten in CSV-Dateien speichern.
- Vor der Nutzung immer eine lokale Sicherung der Originaldaten anlegen.
- CSV-Dateien vor dem Import auf Format und Inhalte prüfen.

## Haftung und Datenschutzhinweis

Diese Web-App ist öffentlich über GitHub Pages verfügbar und nutzt externe Ressourcen. Dadurch können Daten technisch auch über externe Server verarbeitet oder übertragen werden. Die Nutzung erfolgt auf eigenes Risiko.

Für etwaige Datenverluste, fehlerhafte Auswertungen oder sonstige Schäden wird keine Haftung übernommen. Jede nutzende Person ist selbst dafür verantwortlich, nur zulässige Daten zu verwenden und die datenschutzrechtlichen Anforderungen einzuhalten.