# Operative Entscheidungen Playbook

## Übersicht

Dieses Playbook hilft bei operativen Entscheidungen, die den täglichen Betrieb und die Produktentwicklung betreffen.
Operative Entscheidungen sind typischerweise **Type 2 (Two-way door)** - reversibel und experimentell.

## Typische operative Entscheidungen

### Produkt & Features

- Feature-Priorisierung und -Entwicklung
- UI/UX Verbesserungen
- Performance-Optimierungen
- Bug-Fix vs. Feature-Trade-offs

### Technische Infrastruktur

- Tool- und Platform-Wahlen
- Deployment-Strategien
- Monitoring und Alerting
- Datenbank- und Storage-Entscheidungen

### Prozesse & Workflow

- Team-Meeting-Strukturen
- Code-Review-Prozesse
- Testing-Strategien
- Dokumentations-Standards

### Ressourcen-Allokation

- Sprint-Planung und -Priorisierung
- Team-Bandwidth-Verteilung
- Budget-Allokation für Tools/Services
- Zeit-Investition in verschiedene Bereiche

## Prozess für operative Entscheidungen

### 1. Kontext sammeln (1-3 Tage)

**Schnelle Problem-Definition:**

- **Problem-Statement**: Was funktioniert nicht optimal?
- **Betroffene**: Wer leidet unter dem aktuellen Zustand?
- **Messbare Auswirkung**: Wie zeigt sich das Problem in Metriken?
- **Constraints**: Zeit, Budget, technische Grenzen?

**Company Handbuch Alignment:**

- **Speed-to-Learn** (Kapitel 11): Warum nicht jetzt? Klein anfangen, groß lernen
- **Keine Perfektion** (Kapitel 15): Klar + funktionsfähig + dokumentiert
- **PRs > Issues > Slack** (Kapitel 15): Öffentliche Dokumentation bevorzugt

### 2. Optionen erkunden (2-5 Tage)

**Mindestens 3 pragmatische Alternativen:**

- **Quick Fix**: Minimaler Aufwand, schneller Impact
- **Proper Solution**: Nachhaltig, aber aufwändiger
- **Experimental Approach**: Test einer neuen Idee

**Für jede Option dokumentieren:**

- **Aufwand**: Zeit und Ressourcen
- **Impact**: Erwartete Verbesserung
- **Risiko**: Was kann schiefgehen?
- **Trade-offs**: Was müssen wir opfern?

### 3. Impact-Analyse (1-2 Tage)

**Fokussierte Wirkungsbetrachtung:**

**30 Tage:**

- Unmittelbare Verbesserungen für Nutzer:innen/Team
- Erste Metriken-Änderungen
- Schnelle Feedback-Loops

**90 Tage:**

- Etablierte neue Prozesse/Patterns
- Produktivitäts- oder Qualitätsverbesserungen
- Lern-Effekte im Team

**365 Tage:**

- Nachhaltige Verbesserungen
- Kumulativer Business-Value
- Dokumentierte Best Practices

### 4. Entscheidung treffen (1-2 Tage)

**Entscheidungs-Owner:** Produkt-Team oder Technical Lead

**Entscheidungskriterien:**

1. **Impact/Complexity Ratio** (40%): Größter Nutzen mit geringstem Aufwand
2. **Lern-Potential** (30%): Was können wir daraus lernen?
3. **Reversibilität** (20%): Können wir zurückrudern wenn nötig?
4. **Team-Alignment** (10%): Unterstützt das gesamte Team diese Richtung?

### 5. Learning & Iteration (kontinuierlich)

**Review-Kadenz:**

- **30-Tage-Review**: Erste Ergebnisse und Anpassungen
- **90-Tage-Review**: Muster erkennen und optimieren
- **Keine 365-Tage-Reviews**: Operative Entscheidungen werden kontinuierlich angepasst

## Operative Entscheidungs-Kategorien

### Feature-Priorisierung (Kapitel 8 Company Handbuch)

**RFC-Prozess für Features:**

1. **Problem definieren**: Welches Nutzer:innen-Problem löst das?
2. **Lösungsoptionen**: Mindestens 3 verschiedene Approaches
3. **Impact messen**: Wie verbessert sich die Nutzererfahrung?
4. **Implementierung**: Klein anfangen, iterativ erweitern

**Priorisierungskriterien:**

- **Nutzer:innen-Value**: Direkter Nutzen für Endbenutzer:innen
- **Business-Impact**: Beitrag zu Wachstum/Monetarisierung
- **Technische Machbarkeit**: Können wir das umsetzen?
- **Lern-Potential**: Was erfahren wir Neues?

### Technische Architektur (Kapitel 15 Company Handbuch)

**Wann ADR?**

- Architekturell bedeutsame Änderungen
- System-weite Auswirkungen
- Langfristige technische Verschuldung

**Wann kein ADR?**

- Feature-spezifische Implementierungsdetails
- Kleine Optimierungen ohne System-Impact
- Temporäre Workarounds

### Team-Workflows (Kapitel 9, 12 Company Handbuch)

**Async-First Prinzipien:**

- **Dokumentation first**: Alles was wichtig ist, steht schriftlich
- **Fokuszeiten respektieren**: Keine Unterbrechungen in Deep Work
- **Issues statt Slack**: Entscheidungen in GitHub, Koordination in Chat

**Meeting-Optimierung:**

- **Purpose vor Presence**: Jedes Meeting braucht klares Ziel
- **Async vorbereiten**: Material im Voraus teilen
- **Action Items dokumentieren**: Konkrete nächste Schritte

### Ressourcen-Allokation (Kapitel 7, 13 Company Handbuch)

**Budgets:**

- **Dokumentation first**: Inhalte schaffen langfristigen Wert
- **Tools second**: Richtige Tools ermöglichen Effizienz
- **People first**: Talente vor Tools priorisieren

**Zeit-Investition:**

- **Wirkung messen**: Was bringt den größten Impact?
- **Lernen fördern**: Raum für Experimente schaffen
- **Schulden reduzieren**: Technische und Prozess-Schulden aktiv managen

## Schnelle operative Entscheidungen

### 15-Minuten-Entscheidungen

Für kleine, reversible Änderungen:

1. **Problem identifizieren** (2 Minuten)
2. **2-3 Optionen brainstormen** (5 Minuten)
3. **Entscheiden und begründen** (3 Minuten)
4. **Umsetzen** (5 Minuten)

**Beispiele:**

- Button-Farbe ändern
- Fehlermeldung verbessern
- Dokumentations-Update
- Kleine Prozess-Anpassung

### 1-Tages-Entscheidungen

Für mittlere operative Änderungen:

1. **Morgen**: Problem analysieren, Betroffene informieren
2. **Mittag**: Optionen entwickeln, erste Feedback einholen
3. **Abend**: Entscheidung treffen und kommunizieren

## Kommunikation operativer Entscheidungen

### Team-interne Kommunikation

- **GitHub Issues**: Für Entscheidungs-Dokumentation
- **Team-Channel**: Für Awareness und Fragen
- **1:1 Gespräche**: Für direkt Betroffene

### Änderungs-Management

- **Rollout-Plan**: Wie führen wir die Änderung ein?
- **Training**: Braucht das Team Unterstützung?
- **Feedback-Loops**: Wie sammeln wir frühes Feedback?

## Risiko-Management für operative Entscheidungen

### Häufige operative Risiken

1. **Feature Creep**: Features werden größer als geplant
   - **Mitigation**: Klare Scope-Definition, MVP-Ansatz

2. **Team-Überlastung**: Zu viele parallele Initiativen
   - **Mitigation**: Priorisierung nach Impact, regelmäßige Capacity-Checks

3. **Technische Schulden**: Schnelle Lösungen schaffen langfristige Probleme
   - **Mitigation**: Technische Reviews, Refactoring-Plan

4. **Nutzer:innen-Verwirrung**: Änderungen überraschen Nutzer:innen
   - **Mitigation**: Change-Communication, Beta-Tests

## Erfolgs-Beispiele aus der Praxis

### Gute operative Entscheidungen

- **Async-First Kommunikation**: Weniger Meetings, mehr Fokuszeit
- **Issue-basierte Entwicklung**: Bessere Nachvollziehbarkeit von Entscheidungen
- **MVP-first Features**: Schneller Kund:innen-Feedback, weniger Waste

### Vermeidbare Fehler

- **Keine klaren Owner**: Entscheidungen ohne Verantwortliche verzögern sich
- **Perfektion über Speed**: Type 2 Entscheidungen nicht überanalysieren
- **Stakeholder vergessen**: Überraschte Teams blockieren Implementierung

## Tools & Ressourcen

- **Entscheidungsvorschlag Template**: Für strukturierte Vorschläge
- **Impact Scorecard**: Für quantitative Bewertung
- **Retrospective Template**: Für Lessons Learned
- **Team Capacity Tracker**: Für Ressourcen-Planung

### WeMake-spezifische Tools

- **Clarity BI**: Für Daten-gestützte Entscheidungen
- **V41 Platform**: Für operative Workflows
- **GitHub Projects**: Für Entscheidungs-Tracking

## Kontinuierliche Verbesserung

### Regelmäßige Reviews

- **Wöchentliche Retros**: Was können wir besser machen?
- **Monatliche Reviews**: Entscheidungsqualität bewerten
- **Quartalsweise**: Prozess-Optimierungen

### Metriken tracken

- **Decision Velocity**: Zeit von Idee bis Umsetzung
- **Success Rate**: Wie viele Entscheidungen erreichen ihre Ziele?
- **Learning Rate**: Wie schnell passen wir basierend auf Feedback an?

---

_Operative Entscheidungen sind das Herzstück unserer täglichen Arbeit. Sie summieren sich zu strategischem Erfolg._
