# 7 Anforderungen

> Eingeführt in V0.2 (in Arbeit)

Die Anforderungen sind aus dem Event Storming (Kapitel 4) und dem Backlog (Kapitel 6) abgeleitet. Die Spalte «Quelle» zeigt, woher eine Anforderung stammt. So lässt sie sich zurückverfolgen. Die Begriffe sind im Glossar (Kapitel 5) definiert.

**Status:** Alle Anforderungen haben den Status «Entwurf» oder «offen». Keine ist «vereinbart», weil die Ergebnisse aus einem KI-simulierten Workshop stammen (siehe 4.8). Die Status-Werte sind in Kapitel 0.2 erklärt.

**Schreibweise:** Jede Anforderung beginnt mit «Das System muss». Sie enthält genau eine Anforderung und nennt den Akteur. Der Begriff «Das System» steht für CertiKeep.

## 7.1 Funktionale Anforderungen

### Pflichten festlegen

| ID | Anforderung | Quelle | MVP | Status |
|---|---|---|---|---|
| FA-001 | Das System muss der Compliance-Manager:in ermöglichen, für jede Rolle die verlangten Zertifikatsarten festzulegen. | Story 2.3 · Command A | nein | Entwurf |
| FA-002 | Das System muss der Compliance-Manager:in ermöglichen, für jede Zertifikatsart eine Vorwarnfrist in Tagen festzulegen. | Story 1.1 · Event A · H2 | ja | Entwurf |
| FA-003 | Das System muss der Compliance-Manager:in ermöglichen, eine Zertifikatsart als sicherheitskritisch zu kennzeichnen. | Story 2.2 · Policy B · H3 | nein | Entwurf |

### Nachweis erbringen

| ID | Anforderung | Quelle | MVP | Status |
|---|---|---|---|---|
| FA-004 | Das System muss Mitarbeiter:innen ermöglichen, einen eigenen Nachweis mit Zertifikatsart und Ablaufdatum zu erfassen und dabei ein Zertifikat als PDF oder Foto anzuhängen. Bei Zertifikatsarten mit Gesundheitsbezug entfällt das Zertifikat (siehe NFA-003). | Story 2.1 · Command B | ja | Entwurf |
| FA-005 | Das System muss Führungskräften ermöglichen, einen Nachweis für eine Mitarbeiter:in ihres Teams zu erfassen. | Story 2.4 · Command B · H1 | nein | Entwurf |
| FA-006 | Das System muss einen neu erfassten Nachweis einer sicherheitskritischen Zertifikatsart der Compliance-Manager:in zur Prüfung vorlegen. | Story 2.2 · Policy B · H3 | nein | Entwurf |
| FA-007 | Das System muss der Compliance-Manager:in ermöglichen, einen zur Prüfung vorgelegten Nachweis freizugeben oder abzulehnen. | Story 2.2 · Command B | nein | Entwurf |
| FA-008 | Das System muss einen neu erfassten Nachweis einer nicht sicherheitskritischen Zertifikatsart sofort auf den Status «gültig» setzen. | H3 | ja | Entwurf |

### Gültigkeit überwachen

| ID | Anforderung | Quelle | MVP | Status |
|---|---|---|---|---|
| FA-009 | Das System muss der Mitarbeiter:in eine E-Mail-Erinnerung senden, sobald ein eigener Nachweis die Vorwarnfrist erreicht. | Story 1.4 · Policy C | ja | Entwurf |
| FA-010 | Das System muss der zuständigen Führungskraft eine E-Mail-Erinnerung senden, sobald ein Nachweis ihres Teams die Vorwarnfrist erreicht. | Story 1.1 · Policy C · H6 | ja | Entwurf |
| FA-011 | Das System muss die Compliance-Manager:in benachrichtigen, wenn ein Nachweis 14 Tage vor dem Ablaufdatum noch nicht erneuert ist. | Story 1.6 · Policy C | nein | Entwurf |
| FA-012 | Das System muss einen Nachweis auf den Status «erneuert» setzen, sobald für dieselbe Mitarbeiter:in ein gültiger Nachweis derselben Zertifikatsart mit späterem Ablaufdatum vorliegt. | Event C «Nachweis erneuert» | ja | Entwurf |
| FA-013 | Das System muss einen Nachweis am Tag nach seinem Ablaufdatum auf den Status «abgelaufen» setzen, wenn keine Erneuerung vorliegt. | Policy C · Event C «Nachweis abgelaufen» | ja | Entwurf |
| FA-014 | Das System muss die Mitarbeiter:in und die zuständige Führungskraft benachrichtigen, wenn ein Nachweis den Status «abgelaufen» erhält. | Policy C | nein | Entwurf |
| FA-015 | Das System muss der Führungskraft eine Übersicht aller Nachweise ihres Teams mit Status und Ablaufdatum anzeigen, sortiert nach Ablaufdatum. | Story 1.5 · Read Model C | ja | Entwurf |
| FA-016 | Das System muss der Führungskraft bei einem abgelaufenen Nachweis einer sicherheitskritischen Zertifikatsart einen Sperrhinweis anzeigen. | H4 | nein | **offen** |

### Audit und Austritt

| ID | Anforderung | Quelle | MVP | Status |
|---|---|---|---|---|
| FA-017 | Das System muss der Compliance-Manager:in ermöglichen, für eine Abteilung einen Audit-Report als PDF zu erstellen. | Story 3.1 · Read Model D | nein | **offen** |
| FA-018 | Das System muss die Nachweisdaten einer ausgetretenen Mitarbeiter:in nach Ablauf der Aufbewahrungsfrist löschen. | Story 3.2 · Policy D · H8 | nein | **offen** |

**Noch ohne funktionale Anforderung:** Die Stories 1.2 (Hinweis im Dashboard) und 1.3 (Push-Nachricht) gehören nicht zum MVP. Sie werden spezifiziert, sobald klar ist, ob es einen zweiten Kanal neben der E-Mail braucht (siehe A-03, H6).

## 7.2 Nicht-funktionale Anforderungen

Jede nicht-funktionale Anforderung nennt Kontext, Messgrösse und Schwelle. Die Schwerpunkte kommen aus der Compliance-Welt: Zuverlässigkeit, Nachvollziehbarkeit, Datenschutz und Auditfähigkeit.

| ID | Kategorie | Anforderung | Kontext | Messgrösse | Schwelle | Quelle | Status |
|---|---|---|---|---|---|---|---|
| NFA-001 | Zuverlässigkeit | Das System muss jede fällige Erinnerung zuverlässig versenden. | Normalbetrieb, gemessen über einen Kalendermonat | Anteil der Erinnerungen, die spätestens 24 Stunden nach Erreichen der Vorwarnfrist versendet sind | ≥ 99,9 % | H6 · FA-009, FA-010 | Entwurf |
| NFA-002 | Nachvollziehbarkeit | Das System muss jede Änderung an einem Nachweis mit Zeitpunkt und handelnder Person protokollieren. | Erfassen, Prüfen, Freigeben, Ablehnen und Löschen eines Nachweises | Anteil der Änderungen mit vollständigem Protokolleintrag | 100 % | Event B «Nachweis freigegeben» · Compliance-Manager:in | Entwurf |
| NFA-003 | Datenschutz | Das System muss bei Zertifikatsarten mit Gesundheitsbezug nur das Ergebnis und das Ablaufdatum speichern. | Arbeitsmedizinische Tauglichkeit und vergleichbare Zertifikatsarten | Anzahl gespeicherter Befunde oder Befunddokumente | 0 | H5 · A-04 | Entwurf |
| NFA-004 | Datenschutz | Das System muss einer Führungskraft nur die Nachweise ihres eigenen Teams anzeigen. | Zugriff über alle Ansichten und Exporte | Anteil der abgewiesenen Zugriffe auf Nachweise fremder Teams im Berechtigungstest | 100 % | Datenschutzberater:in · FA-015 | Entwurf |
| NFA-005 | Auditfähigkeit | Das System muss einen Audit-Report rasch bereitstellen. | Abteilung mit bis zu 500 Nachweisen, Normalbetrieb | Zeit vom Auslösen bis zum fertigen PDF | ≤ 60 Sekunden in 95 % der Fälle | Read Model D · FA-017 | Entwurf |
| NFA-006 | Benutzbarkeit | Das System muss das Erfassen eines Nachweises auf dem Smartphone ermöglichen. | Mitarbeiter:in oder Führungskraft ohne Computerarbeitsplatz, ohne Anleitung | Anteil der Testpersonen, die einen Nachweis in höchstens 2 Minuten erfassen | ≥ 90 % | H1 · FA-004, FA-005 | Entwurf |
| NFA-007 | Nachvollziehbarkeit | Das System muss Protokolleinträge vor Änderung und Löschung schützen. | Alle Benutzerrollen, auch die IT-Administrator:in | Anteil der erfolgreichen Änderungs- oder Löschversuche im Sicherheitstest | 0 % | Compliance-Manager:in · NFA-002 | Entwurf |

**Woher die Schwellen kommen:** Die Werte sind begründete Schätzungen der Projektgruppe. Sie sind noch nicht mit Stakeholdern abgestimmt. Die Schwellen von NFA-002, NFA-003, NFA-004 und NFA-007 folgen aus der Art der Anforderung: Ein Protokoll mit Lücken oder ein einziger gespeicherter Befund wäre bereits ein Verstoss.

## 7.3 Qualitätsszenarien

Zwei nicht-funktionale Anforderungen sind zusätzlich als Qualitätsszenario beschrieben.

**QS-01 zu NFA-001 (Zuverlässigkeit der Erinnerung)**

| Element | Inhalt |
|---|---|
| Quelle | Zeitsteuerung von CertiKeep |
| Auslöser | Ein Staplerausweis erreicht die Vorwarnfrist |
| Umgebung | Normalbetrieb, gleichzeitig erreichen 50 Nachweise die Vorwarnfrist |
| Artefakt | Benachrichtigungsdienst |
| Antwort | CertiKeep sendet je eine E-Mail an die Mitarbeiter:in und an die Führungskraft |
| Schwelle | Versand spätestens 24 Stunden nach Erreichen der Vorwarnfrist, in ≥ 99,9 % der Fälle pro Monat |

**QS-02 zu NFA-005 (Auditfähigkeit)**

| Element | Inhalt |
|---|---|
| Quelle | Compliance-Manager:in |
| Auslöser | Eine externe Auditor:in kündigt ein Audit an. Die Compliance-Manager:in löst den Audit-Report aus. |
| Umgebung | Abteilung Lager mit 500 Nachweisen, Normalbetrieb |
| Artefakt | Reporting |
| Antwort | CertiKeep erstellt den Audit-Report als PDF |
| Schwelle | ≤ 60 Sekunden in 95 % der Fälle |

## 7.4 Offene Anforderungen

Drei Anforderungen haben den Status «offen». Zu jeder gehört eine klare Frage.

| ID | Frage | Wen fragen | Bezug |
|---|---|---|---|
| FA-016 | Soll CertiKeep bei einem abgelaufenen sicherheitskritischen Nachweis einen Sperrhinweis anzeigen? Oder bleibt die Entscheidung, ob jemand weiterarbeiten darf, ganz ausserhalb des Systems? | HR, Geschäftsleitung | H4 |
| FA-017 | Welche Angaben muss der Audit-Report enthalten, und in welcher Form verlangen ihn die externen Auditor:innen? | Externe Auditor:in, Compliance-Manager:in | EZ-03 |
| FA-018 | Wie lange müssen Nachweisdaten nach dem Austritt einer Mitarbeiter:in aufbewahrt werden? | Datenschutzberater:in, Compliance-Manager:in | EZ-03, H8 |

Weitere offene Punkte, die noch keine eigene Anforderung haben:

- **Standard der Vorwarnfrist (EZ-01):** Die Simulation nennt 60 bis 90 Tage für kursgebundene Zertifikatsarten. Das muss eine echte Führungskraft bestätigen.
- **Zweiter Kanal für Erinnerungen (A-03, H6):** Reicht die E-Mail an die Führungskraft, oder braucht es für Mitarbeiter:innen ohne Firmen-E-Mail einen zweiten Kanal, zum Beispiel SMS?
- **Frist der Eskalation (FA-011):** Die 14 Tage stammen aus der Simulation und sind nicht abgestimmt.
