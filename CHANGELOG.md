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
| Cluster-Vertiefung aus dem Repository entfernt | 99.1 | Einzelleistung, gehört nicht ins Gruppen-Pflichtenheft |
| Stakeholdermap auf neun Stakeholder erweitert, mit Einfluss, Interesse und Quadrant | 3.1, 3.2 | Pflichtinhalt Block 2 (KR-14 bis KR-16) |
| Drei Ermittlungsziele und fünf Annahmen mit Risiko ergänzt | 3.3, 3.4 | Pflichtinhalt Block 2 (KR-17, KR-18, KR-20) |
| Neues Kapitel 0: ID-Schema, Status, Baselines und Umgang mit Änderungen | 0.1 bis 0.4 | Pflichtinhalt Block 2 (KR-19, KR-20) |
| Neues Kapitel 4: Event Storming als Ermittlungstechnik, KI-simuliert | 4.1 bis 4.8 | Ermittlung zu EZ-01 und EZ-02 (KR-10, KR-21, KR-23) |
| Board und Vortragsansicht zum Event Storming als Webseiten | event-storming/ | Referat und Abgabe (KR-22, KR-24, KR-25) |
| Verweis auf das entfernte Kapitel 99 ersetzt | 6.1 | Toter Verweis |

### Noch offen bis zur Baseline V0.2

- Glossar mit mindestens acht Begriffen (Kapitel 5). Die Begriffe aus dem Event Storming liegen bereit (siehe 4.7).
- Mindestens sechs funktionale und vier nicht-funktionale Anforderungen mit IDs (Kapitel 7). Die Kandidaten aus dem Event Storming liegen bereit (siehe 4.7).
- Mindestens zwei Anforderungen als «offen» mit klarer Frage. Kandidaten sind H4 (Sperre nach Ablauf) und H8 (Aufbewahrungsdauer).
- Offene Story-Lücke aus KR-11
- Optional: Sicht der Führungskraft mit einer echten Person prüfen (siehe 4.8)
- Ein-Satz-Änderungsnotiz und Tag `v0.2` beim Setzen der Baseline
