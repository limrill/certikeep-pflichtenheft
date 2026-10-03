# 99 Cluster-Vertiefungen (Einzelleistungen)

> Eingeführt in V0.1 · zuletzt geändert in V0.2 (in Arbeit)

## 99.1 Cluster-Vertiefung am Semesterprojekt: Simon Tresch

### Einleitung / Themenwahl

Ich wähle hier Cluster B (Scrum & Backlog), da für mich unklar blieb, wie aus einem statischen Pflichtenheft eine dynamische Sprint-Planung abgeleitet wird. Zwar sind die Grundlagen von Scrum bekannt, die konkrete Schnittmenge aus Kapazitätsplanung, Story-Splitting und Sprint-Ziel-Definition im Rahmen von CertiKeep stellt mich jedoch vor Herausforderungen. Dieser Cluster adressiert genau diese methodische Lücke vor Block 2.

### Vertiefung

In der PVA lag das Hauptproblem darin, dass ich die Sprint-Planung als reines „Abarbeiten von Backlog-Tickets“ missverstanden habe. Für unser Programm bedeutet die richtige Anwendung von Cluster B, dass jeder Sprint durch ein klares Sprint-Goal gesteuert wird und nicht nur durch eine Ansammlung von User Stories. Dies habe ich zuvor nicht verstanden.

Im ersten Entwicklungs-Sprint soll das Ziel beispielsweise lauten: „Compliance-Manager:innen können Zertifikatsdaten erfassen und ablaufende Nachweise im Dashboard visuell erkennen.“

Um dieses Ziel im Planning verlässlich zusagen zu können, müssen wir im Backlog Refinement das Story-Splitting schärfen. Gross geschnittene Anforderungen wie „Erinnerungssystem für ablaufende Zertifikate“ lassen sich nicht in einem Sprint planen. Wir zerlegen dieses Feature für CertiKeep vertikal:

- **Sprint-Beitrag A:** Automatische Identifikation ablaufender Zertifikate in der Datenbank (Backend-Logik).
- **Sprint-Beitrag B:** Benachrichtigungs-Trigger versendet eine Standard-E-Mail 30 Tage vor Ablauf (Integration).
- **Sprint-Beitrag C:** Konfiguration der Fristen durch die IT-Administrator:in (UI).

Durch diese Differenzierung verhindern wir, dass im Sprint-Planning ungeklärte Abhängigkeiten oder unschätzbare Aufwände übernommen werden. Unsere Planung ändert sich dahingehend, dass wir vor jedem Sprint-Planning eine strikte Definition of Ready (DoR) anlegen: Eine Story wird erst eingeplant, wenn Akzeptanzkriterien im Given-When-Then-Format vorliegen und der fachliche Wert für CertiKeep eindeutig ist.

### Fehlannahme

**Fehlannahme:** Das Sprint-Planning dient primär dazu, die obersten Stories aus dem Product Backlog in den nächsten Sprint zu schieben.

**Korrektur (1 Satz):** Falsch, denn das Sprint-Planning startet mit der Definition eines wertgetriebenen Sprint-Ziels, wie die visuelle Warnung ablaufender Nachweise bei der App, und wählt erst danach die fachlich dazu passenden Stories aus.

### Transfer ins Pflichtenheft

- **DoR-Konsens:** Aufnahme von konkreten Kriterien für die Sprint-Bereitschaft von User Stories (z. B. GWT-Kriterien vorhanden).
- **Backlog-Schnitt:** Überarbeitung der Story-Grössen im Backlog für Zertifikats-Upload und Fristenwarnung (Verkleinerung auf sprintfähige Häppchen).
- **Sprint-Ziel-Mapping:** Ergänzung einer Zuordnungs-Spalte im Backlog, welches Feature zu welchem geplanten Sprint-Goal beiträgt.
- **Review-Rhythmus:** Festlegung eines festen Takts für Backlog Refinements vor den jeweiligen Baseline-Releases (V0.1 → V0.2).
- **KI-Review-Spur:** Dokumentation der KI-Vorschläge zur Zerlegung von zu grossen Stories (z. B. Aufteilung von FA-001).
