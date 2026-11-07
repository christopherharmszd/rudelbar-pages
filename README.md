# Rudelbar: Produktionsveröffentlichung

Dieses Repository enthält ausschließlich die Veröffentlichungssteuerung für https://rudelbar.de/. Der bearbeitbare Quellcode liegt in [christopherharmszd/rudelbar-2.0](https://github.com/christopherharmszd/rudelbar-2.0).

`.github/workflows/production.yml` lädt den ausdrücklich freigegebenen Quellcode-Commit, baut und prüft `app/` und veröffentlicht `app/dist/production` über GitHub Pages. Domain, öffentliche Inhalte und CMS-Zugänge bleiben unverändert.

Die alten statischen Dateien im Repository-Stamm wurden am 7. November 2026 entfernt. Sie waren seit der Umstellung auf den Quellcode-Bau kein Veröffentlichungsstand mehr und dürfen nicht als Entwicklungsgrundlage verwendet werden. Frühere Dateien bleiben in der Git-Historie.

## Neues Release

Im Produktionsworkflow den vollständigen Quellcode-SHA sowohl bei `with.ref` als auch bei `RUDELBAR_SOURCE_SHA` setzen. Vorher Quelle, Live-Stand, Testwebsite und Tests prüfen. Nach einem ausdrücklich beauftragten Release erfolgreichen Bau/Deployment und https://rudelbar.de/site-manifest.json kontrollieren.

Der vorhandene Zeitplan übernimmt CMS-Inhalte regelmäßig in statische Seiten. Ein späterer Quellcode-`main`-Push ist keine automatische Produktionsfreigabe. Ein Code-Release überträgt keine CMS-Inhalte zwischen Datasets.

[Veröffentlichungsablauf und Rückweg](https://github.com/christopherharmszd/rudelbar-2.0/blob/main/docs/production-release.md)

Lokaler Checkout: `/Users/christopher.harms/Documents/GitHub/rudelbar-pages`. Die Datei `CNAME` hält die zugehörige Domain sichtbar fest; die eigentliche Website einschließlich ihres CNAME entsteht im Build.
