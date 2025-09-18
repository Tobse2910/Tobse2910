# Portfolio-Übersicht (statische Seite)

Diese kleine statische Seite zeigt ein modernes Design mit Inhaltsverzeichnis und Projekt-Karten. Sie ist sofort nutzbar und leicht anpassbar.

In diesem Repository findest du:

- `index.html` — Hauptseite mit Inhaltsverzeichnis (TOC) und Karten
- `css/styles.css` — Styling mit responsive Grid und modernen Karten
- `data/projects.json` — Beispiel-Projektdaten (einfach editierbar)

## Schnellstart

1. Öffne `data/projects.json` und trage deine Projekte ein. Beispielstruktur für ein Projekt:

   ```json
   {
     "id": "projekt-1",
     "title": "Projekt-Name",
     "description": "Kurzbeschreibung",
     "tags": ["Tag1","Tag2"],
     "url": "https://deine-seite.de/projekt",
     "image": "https://..."
   }
   ```

2. Lokaler Test: Öffne `index.html` direkt im Browser oder starte einen einfachen HTTP-Server (empfohlen):

   ```powershell
   python -m http.server 8000
   # dann im Browser: http://localhost:8000
   ```

## Anpassungen

- Der Footer-Link ist standardmäßig `https://example.com`. Du kannst ihn in `index.html` anpassen oder in `data/projects.json` ein Feld `"site"` setzen.
- Bilder sind in den Beispielen extern verlinkt (Unsplash). Du kannst eigene Bilder lokal ablegen und den Pfad angeben.

## Weiteres

- Möchtest du Filter, Sortierung, Modal-Details oder eine GitHub-Integration, kann ich das ergänzen.
- Wenn du mir die URL deiner Website und ein paar Projekt-Details gibst, aktualisiere ich `projects.json` für dich.

Viel Erfolg!
