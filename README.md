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

## Deployment / Upload

Du kannst die Seite sehr einfach hosten:

- GitHub Pages (empfohlen): Repository in GitHub pushen, in den Repository-Einstellungen GitHub Pages aktivieren (Branch `main`, Root) — die Seite ist dann unter `https://<dein-nutzername>.github.io/<repo>` erreichbar.
- FTP / Webspace: Lade die Dateien (`index.html`, `profile.html`, `css/`, `data/`) in dein Webroot hoch.

Assets & Favicon
- Lege ein `favicon.ico` ins Root-Verzeichnis oder passe den Link im `index.html` an.
- Wenn du Hotlinking vermeiden willst, lade die Bilder aus `data/projects.json` in dein Webspace-Verzeichnis (z. B. `public/`) und passe die `image`-Pfadwerte an.

Automatisches Deployment

- Dieses Repository enthält eine GitHub Actions Workflow-Datei `.github/workflows/pages.yml`, die bei jedem Push auf `main` den Inhalt in den Branch `gh-pages` pusht. Du kannst GitHub Pages so einstellen, dass es die Seite vom Branch `gh-pages` bedient, oder die Aktion anpassen.


