# 6 Backlog

> Eingeführt in V0.1 · zuletzt geändert in V0.2 (in Arbeit)

## 6.1 Initiale Zerlegung

Stories mit dem Vermerk **(MVP)** gehören zum MVP aus 1.2. Stories mit dem Vermerk **(neu in V0.2)** stammen aus dem Event Storming (Kapitel 4).

**Epic: Zertifikats-Lebenszyklusverwaltung & Compliance-Sicherung**

- **Feature 1: Automatisiertes Ablauf- & Benachrichtigungssystem**
  - **User Story 1.1 (MVP):** Als Führungskraft möchte ich automatische E-Mail-Erinnerungen vor dem Ablauf von Zertifikaten meines Teams erhalten, damit Schulungen und Erneuerungen rechtzeitig geplant werden können.
  - **User Story 1.2:** Als Mitarbeiter:in möchte ich im Dashboard einen Hinweis sehen, wenn ein eigenes Zertifikat innerhalb der Vorwarnfrist abläuft, damit ich den Nachweis rechtzeitig aktualisieren kann.
  - **User Story 1.3:** Als Mitarbeiter:in möchte ich eine Push-Nachricht erhalten, wenn ein eigenes Zertifikat innerhalb der Vorwarnfrist abläuft, damit ich auch ohne Blick ins Dashboard davon erfahre.
  - **User Story 1.4 (MVP, neu in V0.2):** Als Mitarbeiter:in möchte ich eine E-Mail-Erinnerung erhalten, wenn ein eigener Nachweis die Vorwarnfrist erreicht, damit ich mich rechtzeitig um die Erneuerung kümmern kann.
  - **User Story 1.5 (MVP, neu in V0.2):** Als Führungskraft möchte ich eine Übersicht aller Nachweise meines Teams mit Status und Ablaufdatum sehen, damit ich fällige Erneuerungen auf einen Blick erkenne.
  - **User Story 1.6 (neu in V0.2):** Als Compliance-Manager:in möchte ich benachrichtigt werden, wenn ein Nachweis kurz vor dem Ablaufdatum noch nicht erneuert ist, damit ich eingreifen kann, bevor er abläuft.
- **Feature 2: Dokumenten- & Zertifikats-Verwaltung**
  - **User Story 2.1 (MVP):** Als Mitarbeiter:in möchte ich neue Zertifikate (PDF/Bild) hochladen und mit Ablaufdatum versehen können, damit meine Qualifikationen im System hinterlegt sind.
  - **User Story 2.2:** Als Compliance-Manager:in möchte ich ausstehende Uploads von Zertifikaten prüfen und freigeben, um sicherzustellen, dass nur gültige und korrekte Dokumente im System erfasst werden.
  - **User Story 2.3 (neu in V0.2):** Als Compliance-Manager:in möchte ich pro Rolle festlegen, welche Zertifikatsarten nötig sind, damit CertiKeep weiss, welche Nachweise jede Mitarbeiter:in braucht.
  - **User Story 2.4 (neu in V0.2):** Als Führungskraft möchte ich Zertifikate für Mitarbeiter:innen meines Teams erfassen können, damit auch Personen ohne Computerarbeitsplatz gültige Nachweise haben.
- **Feature 3: Audit- & Reporting-Engine**
  - **User Story 3.1:** Als Compliance-Manager:in möchte ich mit wenigen Klicks einen vollständigen Audit-Report für eine Abteilung exportieren (PDF/Excel), um bei externen Prüfungen sofort nachweisfähig zu sein.
  - **User Story 3.2 (neu in V0.2):** Als Datenschutzberater:in möchte ich, dass Nachweisdaten ausgetretener Mitarbeiter:innen nach Ablauf der Aufbewahrungsfrist gelöscht werden, damit CertiKeep keine Personendaten länger als nötig aufbewahrt.

**Vorwarnfrist:** Zeitraum vor dem Ablaufdatum, in dem CertiKeep erinnert. Die Compliance-Manager:in legt sie pro Zertifikatsart fest (siehe Glossar und FA-002). Der Standard von 30 Tagen ist noch offen. Das Event Storming deutet auf 60 bis 90 Tage für kursgebundene Zertifikatsarten hin (siehe 4.6, EZ-01).

**Hinweis zur Nummerierung:** Story 1.3 wurde in V0.2 aus der ursprünglichen Story 1.2 abgetrennt. Bestehende Nummern bleiben unverändert (siehe KI-Review-Spur, KR-03).

**Geschlossen in V0.2:** Die E-Mail-Erinnerung an Mitarbeiter:innen und die Übersichtsliste aus dem MVP haben jetzt eigene Stories (1.4 und 1.5). Damit ist die Lücke aus KR-11 geschlossen.

**Hinweis zu den Begriffen:** Die Stories 1.1 bis 3.1 stammen aus V0.1. Sie verwenden noch «Zertifikat», wo das Glossar heute «Nachweis» sagt. Die Wortwahl wird in V0.3 vereinheitlicht, wenn die Stories Akzeptanzkriterien erhalten.
