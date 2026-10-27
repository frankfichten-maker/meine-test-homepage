# Länder-Ranking – JSON-Version

## Dateien
- `index.html`: Webseite und Bewertungslogik
- `data/ranking.json`: Ausgangsdaten der Länder

## Hochladen auf GitHub
1. Öffne dein bestehendes GitHub-Repository.
2. Lade die neue `index.html` hoch und ersetze die vorhandene Datei.
3. Erstelle im Repository einen Ordner `data` (beim Hochladen der Datei kann GitHub den Ordner automatisch anlegen).
4. Lade `ranking.json` in den Ordner `data` hoch.
5. Warte, bis Vercel den neuen Stand deployed hat, und öffne deine Webseite.

Die Ordnerstruktur muss genau so aussehen:
```
index.html
data/ranking.json
```

## Länder bearbeiten
Öffne `data/ranking.json` auf GitHub und bearbeite `name`, `flag`, `likes` oder `dislikes`.
Achte auf gültiges JSON: doppelte Anführungszeichen verwenden und keine Kommas nach dem letzten Eintrag.

## Wichtig
Die Webseite lädt die Ausgangsdaten aus der JSON-Datei. Bewertungen werden weiterhin nur im Browser des jeweiligen Besuchers gespeichert (`localStorage`). Besucher können die Datei auf GitHub nicht direkt ändern; dadurch werden Stimmen noch nicht gemeinsam für alle gespeichert.

Wenn du die Webseite direkt als lokale Datei öffnest (`file://`), kann der Browser das Laden der JSON-Datei blockieren. Teste daher über Vercel oder einen lokalen Webserver.


## Balkenberechnung
Die Balken werden unabhängig pro Land berechnet. Eine Bewertung für Japan verändert nicht mehr die Balkenbreite der anderen Länder.
