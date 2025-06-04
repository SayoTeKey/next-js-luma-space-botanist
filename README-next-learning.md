# favicon

wohin speichern?
Gute Frage!
Mit dem neuen Next.js App Router (ab Next.js 13) gibt es zwei Möglichkeiten, Favicons und andere Metadaten zu verwalten:

1. Favicon im app-Ordner
   Wenn du ein neues Next.js-Projekt mit dem App Router startest, findest du oft eine Datei wie favicon.ico, icon.png oder apple-touch-icon.png direkt im app-Ordner.
   Das liegt daran:

Next.js erkennt spezielle Dateien (icon.png, apple-touch-icon.png, favicon.ico) im jeweiligen Routen-Ordner (app oder Unterordner) automatisch und bindet sie für diese Route als Favicon ein.
Das ist praktisch, wenn du für verschiedene Routen unterschiedliche Favicons haben möchtest. 2. Favicon im public-Ordner
Traditionell (und auch weiterhin unterstützt) werden statische Dateien wie das Favicon im public-Ordner abgelegt.
Vorteile:

Die Datei ist immer unter /favicon.ico erreichbar, egal auf welcher Route du bist.
Viele Tools, Browser und Crawler erwarten das Favicon genau an dieser Stelle.
Es ist die kompatibelste und einfachste Lösung, besonders wenn du nur ein Favicon für die ganze Seite brauchst.
Warum solltest du dein eigenes Favicon in den public-Ordner legen?
Kompatibilität: Manche Browser und externe Dienste suchen das Favicon explizit unter /favicon.ico.
Einfachheit: Du musst keine Metadaten oder spezielle Next.js-Features nutzen, sondern kannst einfach die Datei ersetzen.
Globale Gültigkeit: Das Favicon gilt für die gesamte Seite, nicht nur für eine Route.
Fazit
Für ein globales Favicon: Lege es in den public-Ordner.
Für route-spezifische Favicons: Lege sie in den jeweiligen app-Unterordner.
Tipp:
Wenn du nur ein Favicon für die ganze Seite willst, ist der public-Ordner der sicherste und einfachste Weg!
