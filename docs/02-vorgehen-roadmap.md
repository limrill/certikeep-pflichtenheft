# 2 Vorgehen und Artefakt-Roadmap

> Eingeführt in V0.1 · zuletzt geändert in V0.2 (in Arbeit)

## 2.1 Vorgehensannahme: Hybrid

| Vorgehen | Was | Begründung |
|---|---|---|
| Plangetrieben | Vision, Pflichtenheft V0.1 – V1.0, Architektur | Teil der Semesterarbeit, einzelne Etappen sind vorgegeben |
| Agil | 4-Wochen-Sprints, Backlog-Refinement, Sprint-Reviews mit Stakeholder-Sample | die Realisierung selbst läuft agil, um Stakeholder-Feedback einzubinden. |

## 2.2 Artefakte Roadmap

| Block / Datum | Artefakt | Beschreibung | Wer |
|---|---|---|---|
| Block 1 (V0.1) · 07.09.2026 | Vision · Stakeholder-Map · Vorgehensmodell · Backlog · MVP-Hypothese | Erste Pflichtenheft-Baseline | Projektgruppe 3 |
| Block 2 (V0.2) · 05.10.2026 | Glossar · Entity-Diagramm · Stories mit AK · FAs · NFAs · Qualitätsszenarien · Interview-Auswertung | Anforderungs-Tiefe + Stakeholder-Substanz | Projektgruppe 3 |
| Block 3 (V0.3) · 02.11.2026 | UC-Übersicht · Haupt-UC vollständig · UC-Diagramm · NFA-AK (SMART) · KI-Review · DoR/DoD | Use-Case-Detail + testbare AK | Projektgruppe 3 |
| Block 4 (V0.4) · 30.11.2026 | CRC · BCE · Klassendiagramm · Sequenz-/Zustand-/Aktivitätsdiagramm · Haupt-ADR · KI-Review | Lösungs-Substanz | Projektgruppe 3 |
| Block 5 (V0.5) · 14.12.2026 | Qualitäts-Audit · Given–When–Then-Kriterien · Testideen mit Teststufe · erweiterte Traceability · Einführung und Betrieb · Abschluss-Checkliste · Selbstbeurteilung | Geprüfte, nachweisbare Spezifikation | Projektgruppe 3 |
| Abgabe (V1.0) · 14.12.2026 | Offene Stellen geschlossen oder begründet · Änderungsprotokoll abgeschlossen | Abgabefassung | Projektgruppe 3 |

## 2.3 Eine bewusste Lücke

**Lücke:** Die Anbindung an HR-Software und an einen Identity Provider (SSO).

**Was wir jetzt festhalten:** Nur das Interesse der IT-Administrator:in (siehe 3.1). Im MVP werden Mitarbeiter:innen per Liste oder CSV-Import erfasst.

**Warum später:** Das MVP soll prüfen, ob automatische Erinnerungen wirken (siehe 1.2). Dafür braucht es keine Integration. Eine Integration ist aufwendig und hängt von den Systemen der Auftraggeberin ab. Sie lohnt sich erst, wenn die MVP-Hypothese bestätigt ist.

**Wann:** Die Schnittstellen werden in der Architektursicht beschrieben (Block 4, V0.4). Umgesetzt werden sie frühestens nach dem Pilot.

