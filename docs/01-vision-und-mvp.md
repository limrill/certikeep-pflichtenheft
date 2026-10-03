# 1 Vision und MVP

> Eingeführt in V0.1 · zuletzt geändert in V0.2 (in Arbeit)

## 1.1 Projekt in einem Absatz / Vision

Unternehmen halten ihre gesetzlichen und betrieblichen Qualifikations- und Sicherheitsnachweise jederzeit lückenlos ein, ohne manuellen Nachverfolgungsaufwand. CertiKeep stellt sicher, dass Mitarbeitende und Führungskräfte ablaufende Zertifikate rechtzeitig erkennen und erneuern, sodass Organisationen in Audits voll handlungs- und nachweisfähig bleiben.

## 1.2 MVP-Hypothese

Die MVP-Hypothese folgt dem Schema Outcome-Hypothese → MVP → Messung → Entscheid. Sie ersetzt die Fassung aus V0.1 (Begründung in der KI-Review-Spur, KR-05).

### Outcome-Hypothese

Wenn Mitarbeiter:innen und ihre Führungskraft automatisch vor dem Ablauf eines Zertifikats erinnert werden, wird der Nachweis rechtzeitig erneuert.

### MVP

Ein Pilot in einer Abteilung mit 20 bis 40 Mitarbeiter:innen.

**Im MVP enthalten:**

- Zertifikate mit Ablaufdatum erfassen (Story 2.1)
- E-Mail-Erinnerung vor dem Ablauf an Führungskraft (Story 1.1) und Mitarbeiter:in
- Übersichtsliste aller Zertifikate der Abteilung

**Bewusst nicht im MVP enthalten:**

- Freigabe durch Compliance-Manager:innen (Story 2.2)
- Audit-Report (Story 3.1)
- Push-Nachrichten (Story 1.3)
- Anbindung an HR-Software und SSO (siehe bewusste Lücke, 2.3)

### Messung

| Schritt | Inhalt |
|---|---|
| Ausgangslage | Vor dem Pilot wird aus der bisherigen Nachweisliste ermittelt, wie viele Nachweise der Pilotabteilung in den letzten sechs Monaten abgelaufen sind, bevor sie erneuert wurden. |
| Dauer | Drei Monate |
| Messgrösse | Anteil der im Pilotzeitraum fälligen Nachweise, die vor ihrem Ablaufdatum erneuert oder mit einem Schulungstermin eingeplant wurden |
| Schwelle | ≥ 90 % |

**Hypothese:** Im dreimonatigen Pilot werden mindestens 90 % der fälligen Nachweise vor ihrem Ablaufdatum erneuert oder eingeplant. Die Ausgangslage dient als Vergleich. Sie zeigt, wie gross die Verbesserung gegenüber heute ist.

### Entscheid nach dem MVP

- **Hypothese bestätigt:** CertiKeep wird ausgebaut. Als Nächstes folgen die Freigabe durch Compliance-Manager:innen und der Audit-Report.
- **Hypothese nicht bestätigt:** Zurück in die Discovery. Zu klären ist, ob die Erinnerung nicht wirkt oder ob Schulungstermine fehlen.
