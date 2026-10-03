# Änderungsverzeichnis

Jede Baseline ist im Repository als Git-Tag gesetzt. Die Tabelle nennt pro Version, was dazukam und warum. Die IDs KR-xx verweisen auf die [KI-Review-Spur](ki-review-spur.md).

| Version | Datum | Block | Wer | Was wurde ergänzt oder geändert | Begründung |
|---|---|---|---|---|---|
| V0.1 | 07.09.2026 | 1 | Projektgruppe 3 | Vision · Stakeholder · Vorgehensmodell · Artefakt-Roadmap · Backlog · MVP-Hypothese · Cluster-Vertiefung | Erste Pflichtenheft-Baseline. Abgegeben als PDF, ins Repository übertragen am 03.10.2026 (Tag `v0.1`). |
| V0.2 | in Arbeit | 2 | Projektgruppe 3 | siehe unten | Anforderungs-Tiefe und Stakeholder-Substanz |

## V0.2 – Stand der Arbeit

### Bereits umgesetzt

| Was | Betroffene Stelle | Grund |
|---|---|---|
| Pflichtenheft ins Git-Repository überführt, ein Kapitel pro Datei | ganzes Dokument | Docs-as-Code (KR-09) |
| Rollennamen vereinheitlicht | 3.1, 6.1, 99.1 | Konsistenz (KR-01) |
| «DoD-Konsens» zu «DoR-Konsens» korrigiert | 99.1 | Begriff verwechselt (KR-02) |
| Story 1.2 geteilt, neue Story 1.3 | 6.1 | Zwei Anforderungen in einem Satz (KR-03) |
| Vorwarnfrist konfigurierbar statt fix 30 Tage | 6.1 | Widerspruch zu 99.1 (KR-04) |
| MVP-Hypothese neu gefasst | 1.2 | Nicht prüfbar (KR-05) |
| Bewusste Lücke ergänzt | 2.3 | Pflichtinhalt fehlte (KR-06) |
| KI-Review-Spur ergänzt | ki-review-spur.md | Abschnitt war leer |
| Tippfehler korrigiert («Steakholder», «Ablaufsdatum», «missverstanden haben») | 3.1, 6.1, 99.1 | Sprachliche Korrektheit |

### Noch offen bis zur Baseline V0.2

- Stakeholdermap mit mindestens sechs Stakeholdern, eingeordnet nach Einfluss und Interesse
- Drei Ermittlungsziele und eine Annahmenliste mit Risiko
- Event Storming als Ermittlungstechnik (Kapitel 4)
- Glossar mit mindestens acht Begriffen (Kapitel 5)
- Mindestens sechs funktionale und vier nicht-funktionale Anforderungen mit IDs (Kapitel 7)
- ID-Schema und Ein-Satz-Änderungsnotiz
- Mindestens zwei Anforderungen als «offen» mit klarer Frage
- Offene Story-Lücke aus KR-11
