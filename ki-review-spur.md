# KI-Review-Spur

Hier steht jeder Vorschlag, den eine KI zum Pflichtenheft gemacht hat. Zu jedem Vorschlag gehören ein Entscheid und eine Begründung. Entschieden hat immer die Projektgruppe.

**Eingesetzte KI:** Claude (Anthropic).

**Kriterien:** Die Nummern in der Spalte «Kriterium» beziehen sich auf die Review-Checkliste aus den SWEM-Arbeitshilfen:

1 Eindeutigkeit · 2 Testbarkeit · 3 Vollständigkeit · 4 Konsistenz · 5 Notwendigkeit · 6 Verfolgbarkeit · 7 Messbarkeit · 8 Umsetzbarkeit

Ein Strich (–) bedeutet: Der Vorschlag betrifft das Vorgehen oder die Struktur, nicht eine einzelne Anforderung.

**Entscheide:** übernommen · teilweise · verworfen · offen

**Rolle der KI:** Die KI hat nicht nur geprüft, sondern bei KR-05 und KR-06 auch den Text vorgeschlagen. Die Projektgruppe hat diese Texte geprüft und übernommen.

## V0.0 → V0.1

In der Fassung V0.1 wurde keine KI eingesetzt. Der Abschnitt blieb in der Abgabe deshalb leer.

## V0.1 → V0.2

Review der Fassung V0.1 am 03.10.2026.

| ID | KI-Vorschlag | Kriterium | Entscheid | Begründung |
|---|---|---|---|---|
| KR-01 | Rollennamen vereinheitlichen. V0.1 nennt vier Bezeichnungen für zwei Rollen («Compliance & Audit Manager», «Compliance Manager», «Teamleiter», «Führungskräfte»). | 4 | übernommen | Vier verbindliche Rollen in 3.1 festgelegt. Das Glossar in V0.2 baut darauf auf. |
| KR-02 | In der Cluster-Vertiefung «DoD-Konsens» durch «DoR-Konsens» ersetzen. | 4 | übernommen | Gemeint sind Kriterien für die Sprint-Bereitschaft. Das ist die Definition of Ready. |
| KR-03 | Story 1.2 in zwei Stories teilen: Hinweis im Dashboard und Push-Nachricht. | 1 | übernommen | Ein Satz enthielt zwei Anforderungen (Anti-Pattern 3). Die neue Story erhält die Nummer 1.3. Nummer 1.2 bleibt, weil IDs nie umnummeriert werden. |
| KR-04 | Die feste Frist «30 Tage» in Story 1.2 durch eine konfigurierbare Vorwarnfrist ersetzen. | 4 | übernommen | Widerspruch zur Cluster-Vertiefung, Sprint-Beitrag C (Fristen sind konfigurierbar). Standard bleibt 30 Tage. |
| KR-05 | MVP-Hypothese nach dem Schema Outcome → MVP → Messung → Entscheid neu fassen. Pilot drei Monate statt ein Jahr. Ausgangslage vorher messen. | 2, 7 | übernommen | Die Fassung V0.1 war nicht prüfbar. Ein Jahr ist für ein MVP zu lang, und ohne Ausgangslage fehlt der Vergleich. |
| KR-06 | Als bewusste Lücke die Anbindung an HR-Software und SSO festhalten. | – | übernommen | Pflichtinhalt aus Block 1. Das MVP funktioniert ohne Integration. Sie lohnt sich erst nach bestätigter Hypothese. |
| KR-07 | Alternativ den Audit-Report als bewusste Lücke wählen. | – | verworfen | Die Integration hat den klareren Bezug zu einem Stakeholder-Interesse (IT-Administrator:in). |
| KR-08 | Die Texte der Artefakt-Roadmap eigenständig formulieren, weil sie dem CampusRad-Beispiel stark gleichen. | – | verworfen | Struktur und Inhalte der Roadmap sind im Unterricht vorgegeben. |
| KR-09 | Das Pflichtenheft als Docs-as-Code in einem Git-Repository führen statt in Word. | – | übernommen | Baselines als Git-Tags, Änderungen sind zeilengenau nachvollziehbar, Diagramme ab Block 4 renderbar mit Mermaid. |
| KR-10 | Event Storming als Ermittlungstechnik einsetzen. | – | übernommen | Passt zum Referatsthema der Gruppe. Wird KI-simuliert durchgeführt und als Simulation gekennzeichnet. |
| KR-11 | Das MVP enthält eine E-Mail an Mitarbeiter:innen und eine Übersichtsliste. Dafür gibt es keine Story. | 6 | offen | Wird bei der Überarbeitung des Backlogs in V0.2 geklärt. |
| KR-12 | Nicht-funktionale Anforderungen aus der Compliance-Welt ableiten (Nachvollziehbarkeit, Datenschutz, Zuverlässigkeit der Erinnerung, Auditfähigkeit). | – | übernommen | CertiKeep hat andere Qualitätstreiber als das Modulbeispiel. Umsetzung in Kapitel 7 (V0.2). |
| KR-13 | Den Zertifikats-Lebenszyklus als durchgehendes Zustandsmodell nutzen (Glossar bis Tests). | – | offen | Die Gruppe konzentriert sich vorerst auf KR-09, KR-10 und KR-12. Neu beurteilen nach dem Event Storming. |
