# Rudelbar Produktionswebsite

Die aktive Website https://rudelbar.de/ wird mit .github/workflows/production.yml über GitHub Pages veröffentlicht. Der Workflow baut den ausdrücklich freigegebenen Quellcode-Commit 48ef0309ce26495daaa040658f71329176872f13 aus christopherharmszd/rudelbar-2.0. Die daneben erhaltenen alten statischen Dateien sind ein historischer Rückkehrstand und nicht mehr das aktive Pages-Artefakt.

CMS-Veröffentlichungen lösen einen neuen Build derselben Codeversion mit aktuellen veröffentlichten production-Inhalten aus. Ein Zeitplan dient als Rückfallebene. Kein CMS-Schreibschlüssel und kein GitHub-PAT gehört in dieses öffentliche Repository.

Neue Code-Releases nur durch bewusstes Ändern der festen Quellcode-SHA im Workflow. Staging bleibt getrennt unter rudelbar-2.0. Betriebs- und Rollback-Hinweise stehen im Quellcode unter docs/website-audit-release-2026-11-05.md.
