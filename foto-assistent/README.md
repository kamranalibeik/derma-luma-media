# Foto-Assistent (Derma Luma)

Stand: 2026-11-12

Kleine Web-App fürs Praxis-iPhone: Behandlung wählen, dann Foto für Foto mit Beispielbild und Anweisung durch die Posen. „Foto aufnehmen“ öffnet die iPhone-Kamera, am Ende werden alle Fotos über das Teilen-Menü in der Fotos-App gesichert und danach in Clinicminds hochgeladen.

- Eine Datei (`index.html`), kein Backend, kein Tracking, kein Upload. Fotos liegen nur im Arbeitsspeicher des Tabs.
- Beispielbilder: KI-generierte Fotos (ChatGPT, 09.11. und 12.11.2026, keine echte Person) in `beispiele/`; Illustrationen (SVG im Code) als Rückfall. Keine Patientenfotos in diesem Repo.
- Aufbau (seit 12.11.2026): Startseite mit Hauptkachel „Beratung & Behandlung“ (Standard-Set Gesicht rundherum plus Mimik, 8 Fotos), darunter die Kategorien wie im Buchungsfunnel (`derma-luma-booking/src/config/serviceMapping.ts`) mit ihren Behandlungen. Vorbereitung mit einer einzigen Checkbox. Zoomen und Scrollen sind gesperrt, jeder Schritt passt auf einen Bildschirm (getestet 375×667 und 390×844).
- Posen und Behandlungen: Objekte `P`, `BERATUNG`, `GROUPS` und `FOTOS` in `index.html`. Neue Behandlung im Funnel → hier in `GROUPS` ergänzen. Körperzonen (`body:true`) haben eigene Vorbereitung und einen Ausschnitt-Hinweis (`crop`).
- Installation: Seite in Safari öffnen → Teilen → „Zum Home-Bildschirm“.
