# Lucias Einrichtungsplaner

Stabile, auf dem Android-Tablet getestete Version (22.11.2026): 2D-Raumplan, 3D-Möbelansicht mit 206 Modellen, Farbfelder, 90°-Drehung und ein-/ausblendbare Beschriftungen.

## Veröffentlichung über GitHub Pages
1. Alle sechs Dateien aus diesem Ordner in das **Hauptverzeichnis** des vorgesehenen GitHub-Repositories hochladen (nicht den ZIP-Ordner als Ordner hochladen).
2. Vorhandene `index.html`, `sw.js`, `manifest.webmanifest` und Icons durch diese Version ersetzen; alte, unbenutzte Test-HTML-Dateien müssen nicht veröffentlicht werden.
3. Unter **Settings → Pages** als Quelle **Deploy from a branch**, Branch `main`, Ordner `/(root)` wählen und speichern (falls noch nicht eingerichtet).
4. Die von GitHub angezeigte Pages-Adresse öffnen. Die App kann dort nach dem ersten vollständigen Laden auch offline verfügbar sein.

## Wichtiger Hinweis zu vorhandenen Raumplänen
Raumpläne werden im Browser lokal gespeichert. Die GitHub-Pages-Adresse hat einen anderen Speicherbereich als lokal geöffnete HTML-Dateien. Daher werden bisherige Pläne **nicht automatisch** übernommen. Den bisherigen Raumplan in der alten Version über die vorhandene Sicherungs-/Exportfunktion als JSON sichern und in der veröffentlichten Version über die Importfunktion laden. Diese Schritte sind nur beim Umzug nötig, nicht bei normalen späteren Updates unter derselben Pages-Adresse.

## Technische Hinweise
- Die gesamte App einschließlich der 3D-Möbelmodelle steckt in `index.html`; keine externen Laufzeitbibliotheken.
- `manifest.webmanifest` und die Icons dienen der Installation auf dem Startbildschirm.
- `sw.js` ermöglicht nach erfolgreicher Installation das Offline-Caching. Für neue Versionen den Cache-Namen in `sw.js` ändern.
- Die geprüfte Nutzer-Version wurde inhaltlich **unverändert** als `index.html` übernommen.

## Smartphone-Testversion
Diese Version ergänzt ausschließlich responsive CSS-Regeln im eingebetteten 3D-Viewer. Bitte zunächst auf Smartphone im Hoch- und Querformat testen, bevor die Version als stabil gilt.
