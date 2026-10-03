# CertiKeep — Pflichtenheft

Semesterarbeit im Modul **SWEM (Software Engineering – Modellierung)** an der FFHS, Projektgruppe 3.

CertiKeep ist ein System, mit dem Unternehmen Qualifikations- und Sicherheitsnachweise ihrer Mitarbeitenden verwalten. Es erkennt ablaufende Zertifikate rechtzeitig und hält Organisationen jederzeit auditfähig.

## So ist das Repository aufgebaut

Das Pflichtenheft ist als **Docs-as-Code** geführt. Jedes Kapitel ist eine eigene Markdown-Datei. Ein Kapitel entsteht in dem Block, in dem es gebraucht wird. Spätere Blöcke ändern bestehende Kapitel, statt neue Kopien anzulegen.

| Datei | Inhalt | Eingeführt in |
|---|---|---|
| [`docs/00-arbeitsweise.md`](docs/00-arbeitsweise.md) | ID-Schema, Status, Baselines, Umgang mit Änderungen | V0.2 |
| [`docs/01-vision-und-mvp.md`](docs/01-vision-und-mvp.md) | Vision, MVP-Hypothese | V0.1 |
| [`docs/02-vorgehen-roadmap.md`](docs/02-vorgehen-roadmap.md) | Vorgehensmodell, Artefakt-Roadmap, bewusste Lücke | V0.1 |
| [`docs/03-stakeholder.md`](docs/03-stakeholder.md) | Stakeholdermap, Ermittlungsziele, Annahmen | V0.1 |
| [`docs/06-backlog.md`](docs/06-backlog.md) | Epic → Feature → User Story | V0.1 |
| [`ki-review-spur.md`](ki-review-spur.md) | Alle KI-Vorschläge mit Entscheid und Begründung | V0.1 |
| [`CHANGELOG.md`](CHANGELOG.md) | Änderungsverzeichnis mit allen Baselines | V0.1 |
| [`archiv/`](archiv/) | Original-Abgaben als PDF | V0.1 |

Die Lücken in der Nummerierung sind Absicht. Die Kapitel 04, 05 und 07 folgen in V0.2. Die Nummern bleiben stabil, auch wenn ein Kapitel später dazukommt.

## Baselines und Änderungen

- Jede Baseline ist ein **Git-Tag** (`v0.1`, `v0.2` …).
- Das [`CHANGELOG.md`](CHANGELOG.md) hält pro Baseline fest, was sich geändert hat und warum.
- Den genauen Unterschied zwischen zwei Baselines zeigt GitHub, zum Beispiel unter [`compare/v0.1...main`](https://github.com/limrill/certikeep-pflichtenheft/compare/v0.1...main).
- Jede Datei nennt im Kopf, in welcher Version sie eingeführt und zuletzt geändert wurde.

## Zuordnung zur ursprünglichen Fassung V0.1

Die Abgabe V0.1 war ein einzelnes Dokument (siehe [`archiv/`](archiv/)). Ihre Abschnitte liegen jetzt hier:

| Abschnitt in V0.1 | Neuer Ort |
|---|---|
| 1 Projekt in einem Absatz / Vision | `docs/01-vision-und-mvp.md` → 1.1 |
| 1.1 Stakeholder | `docs/03-stakeholder.md` → 3.1 |
| 2 Vorgehensannahme | `docs/02-vorgehen-roadmap.md` → 2.1 |
| 3 Artefakte Roadmap | `docs/02-vorgehen-roadmap.md` → 2.2 |
| 3.1 Eine bewusste Lücke | `docs/02-vorgehen-roadmap.md` → 2.3 |
| 4 Initiale Zerlegung | `docs/06-backlog.md` → 6.1 |
| 5 MVP-Hypothese | `docs/01-vision-und-mvp.md` → 1.2 |
| 6 KI-Review-Spur V0.0 → V0.1 | `ki-review-spur.md` |
| 7 Cluster-Vertiefung | nicht mehr im Repository (Einzelleistung) |
