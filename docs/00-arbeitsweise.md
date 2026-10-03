# 0 Arbeitsweise: IDs, Baselines und Änderungen

> Eingeführt in V0.2 (in Arbeit)

## 0.1 ID-Schema

Jedes Artefakt, auf das andere Artefakte verweisen, trägt eine stabile ID.

| Präfix | Bedeutung | Format | Beispiel | Ab |
|---|---|---|---|---|
| FA- | Funktionale Anforderung | dreistellig | FA-001 | V0.2 |
| NFA- | Nicht-funktionale Anforderung | dreistellig | NFA-001 | V0.2 |
| EZ- | Ermittlungsziel | zweistellig | EZ-01 | V0.2 |
| A- | Annahme | zweistellig | A-01 | V0.2 |
| KR- | Eintrag der KI-Review-Spur | zweistellig | KR-01 | V0.2 |
| UC- | Use Case | dreistellig | UC-001 | V0.3 |
| AK- | Akzeptanzkriterium | dreistellig | AK-001 | V0.3 |

**User Stories** behalten ihre Nummer im Format «Feature.Laufnummer», zum Beispiel Story 1.3.

**Regeln:**

1. Jede Anforderung erhält ihre ID, sobald sie im Pflichtenheft steht.
2. Die Nummern laufen fortlaufend hoch.
3. **IDs werden nie umnummeriert.** Wird eine Anforderung gestrichen, bleibt ihre Nummer frei. Sie wird nicht neu vergeben. Die Anforderung bleibt mit dem Status «gestrichen» stehen.
4. Jeder Verweis nennt die ID, nicht die Seitenzahl oder den Abschnitt.

## 0.2 Status einer Anforderung

| Status | Bedeutung |
|---|---|
| Entwurf | Die Anforderung ist formuliert, aber noch nicht geprüft. |
| offen | Es gibt eine ungeklärte Frage. Die Frage steht direkt bei der Anforderung. |
| vereinbart | Die Anforderung ist geprüft und von der Projektgruppe akzeptiert. |
| gestrichen | Die Anforderung entfällt. Der Grund steht im Änderungsverzeichnis. |

## 0.3 Baselines

- Eine Baseline ist ein benannter Stand des Pflichtenhefts. Alles danach gilt als Änderung.
- Jede Baseline ist im Repository als **Git-Tag** gesetzt (`v0.1`, `v0.2` …).
- Zu jeder Baseline gehört eine **Ein-Satz-Änderungsnotiz** im [Änderungsverzeichnis](../CHANGELOG.md). Sie nennt Datum, Version und den wichtigsten Inhalt.
- Den Unterschied zwischen zwei Baselines zeigt GitHub zeilengenau, zum Beispiel unter `compare/v0.1...v0.2`.

## 0.4 Umgang mit Änderungen

Ab V0.2 verfolgen wir jede Änderung an einer Anforderung nach. Dafür gelten drei Regeln:

1. **Jede Änderung nennt die betroffenen IDs.** Das gilt für die Commit-Nachricht und für den Eintrag im Änderungsverzeichnis.
2. **Jede Änderung hat einen Grund.** Mögliche Gründe sind ein Review-Befund, eine neue Erkenntnis aus der Ermittlung oder ein Wunsch eines Stakeholders.
3. **Geht eine Änderung auf einen KI-Vorschlag zurück, steht sie zusätzlich in der [KI-Review-Spur](../ki-review-spur.md).** Dort steht auch, ob die Projektgruppe den Vorschlag übernommen oder verworfen hat.

Ab Block 3 wird daraus ein Review-Ablauf mit Peer-Review. In Block 5 entsteht daraus das vollständige Änderungsprotokoll.
