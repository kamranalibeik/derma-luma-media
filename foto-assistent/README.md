# Foto-Assistent (Derma Luma)

Stand: 2026-11-09

Kleine Web-App fürs Praxis-iPhone: Behandlung wählen, dann Foto für Foto mit Beispielbild und Anweisung durch die Posen. „Foto aufnehmen“ öffnet die iPhone-Kamera, am Ende werden alle Fotos über das Teilen-Menü in der Fotos-App gesichert und danach in Clinicminds hochgeladen.

- Eine Datei (`index.html`), kein Backend, kein Tracking, kein Upload. Fotos liegen nur im Arbeitsspeicher des Tabs.
- Beispielbilder: KI-generierte Fotos (ChatGPT, 09.11.2026, keine echte Person) in `beispiele/`; Illustrationen (SVG im Code) als Rückfall. Keine Patientenfotos in diesem Repo.
- Posen und Behandlungen: Objekte `P`, `TREAT` und `FOTOS` in `index.html`.
- Installation: Seite in Safari öffnen → Teilen → „Zum Home-Bildschirm“.
