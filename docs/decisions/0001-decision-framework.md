# ADR 0001: WeMake Entscheidungsrahmen einführen

## Status

**Status**: accepted

**Datum**: 2025-01-14

**Autor**: @AtlasAI-wemake

**Reviewer**: @heyFlorentin

## Kontext

### Problem-Statement

WeMake trifft täglich wichtige Entscheidungen - von strategischen Produktentscheidungen bis hin zu operativen
Feature-Entwicklungen. Ohne einen strukturierten Rahmen:

1. **Intransparenz**: Entscheidungen werden nicht ausreichend dokumentiert oder kommuniziert
2. **Inkonsistenz**: Unterschiedliche Teams verwenden verschiedene Entscheidungsprozesse
3. **Lern-Verlust**: Aus Entscheidungen wird nicht systematisch gelernt
4. **Skalierungsprobleme**: Mit wachsendem Team wird Koordination schwieriger
5. **Fehlende Nachvollziehbarkeit**: Rationale hinter Entscheidungen gehen verloren

### Architektureller Kontext

WeMake entwickelt KI-gestützte Produkte (Clarity BI, V41) und benötigt einen Rahmen, der:

- Mit unserer Open-Source-Kultur harmoniert
- GitHub-nativ ist und unsere bestehenden Prozesse ergänzt
- Die Werte aus dem Company Handbuch verkörpert
- Für verschiedene Entscheidungstypen skalierbar ist

### Stakeholder

Betroffen sind:

- **Entwicklungsteam**: Tägliche operative Entscheidungen
- **Leadership**: Strategische Richtungsentscheidungen
- **Kund:innen**: Produktentscheidungen wirken sich auf Nutzererfahrung aus
- **Community**: Open-Source-Beiträge und Transparenz

### Constraints

- **GitHub-First**: Rahmen muss in GitHub funktionieren
- **Minimaler Overhead**: Nicht mehr Bürokratie als nötig
- **Kulturelle Passung**: Muss zu unserer "Kontext > Kontrolle" Philosophie passen
- **Skalierbarkeit**: Von Solo-Entscheidungen bis zu Team-Entscheidungen
- **Compliance**: Muss DSGVO und Sicherheitsstandards einhalten

## Entscheidung

### Was wir tun

Wir führen einen strukturierten Entscheidungsrahmen ein, der:

1. **Entscheidungstypen** klar kategorisiert (Type 1 vs. Type 2, strategisch vs. operativ)
2. **5-Stufen-Prozess** für systematische Entscheidungsfindung
3. **GitHub-Integration** durch Templates und Automation
4. **ADR-System** für architekturell bedeutsame Entscheidungen
5. **Lern-Framework** mit 30/90/365-Tage Reviews

### Rationale

**Warum dieser Rahmen?**

1. **Alignment mit Company Handbuch**: Verkörpert "Kontext > Kontrolle", Transparenz und "Klein anfangen, groß lernen"

2. **Pragmatisch**: Unterschiedliche Prozesse für unterschiedliche Entscheidungstypen - nicht one-size-fits-all

3. **GitHub-nativ**: Nutzt unsere bestehenden Tools (Issues, PRs, GitHub Actions)

4. **Lern-orientiert**: Jede Entscheidung wird zu einem Lern-Erlebnis mit strukturierten Reviews

5. **Skalierbar**: Funktioniert für Solo-Gründer bis zu wachsendem Team

**Warum nicht andere Ansätze?**

- **Keine schwere Governance**: Vermeidet Bürokratie die Innovation hemmt
- **Keine reinen OKR/Scorecard-Systeme**: Zu rigid für kreative Entscheidungen
- **Keine reinen Wiki-Ansätze**: Brauchen strukturierte Prozesse, nicht nur Dokumentation

## Konsequenzen

### Positive Auswirkungen

1. **Bessere Entscheidungen**: Strukturierter Prozess führt zu durchdachten Entscheidungen
2. **Mehr Transparenz**: Alle können Entscheidungen nachvollziehen und lernen
3. **Schnelleres Lernen**: Systematische Reviews beschleunigen organisationales Lernen
4. **Einfachere Skalierung**: Neue Teammitglieder verstehen schnell, wie Entscheidungen getroffen werden
5. **Stärkere Kultur**: Verstärkt Ownership, Transparenz und Lern-Mindset

### Negative Auswirkungen

1. **Initialer Lernaufwand**: Team muss sich an neue Prozesse gewöhnen
2. **Dokumentationsaufwand**: Mehr Schreibarbeit für Entscheidungen
3. **Potenzielle Verlangsamung**: Strukturierter Prozess könnte schnelleres Handeln bremsen

### Risiken

1. **Overhead-Risiko**: Rahmen könnte zu viel Bürokratie einführen
   - **Mitigation**: Type 2 Entscheidungen sind sehr schlank, regelmäßige Reviews

2. **Nicht-Nutzung**: Team könnte Templates ignorieren
   - **Mitigation**: Automation und Reviews, kontinuierliche Verbesserung

3. **Kultureller Konflikt**: Könnte gegen "Warum nicht jetzt?" Mentalität verstoßen
   - **Mitigation**: Framework betont Speed-to-Learn über Perfektion

### Migrations-Strategie

**Phase 1: Foundation (Woche 1-2)**

- Core Framework Dokumentation erstellen
- ADR System aufsetzen
- Issue Templates implementieren

**Phase 2: Team Adoption (Woche 3-4)**

- Team-Workshop zur Einführung
- Erste Entscheidungen mit Rahmen dokumentieren
- Feedback sammeln und anpassen

**Phase 3: Optimization (Woche 5-8)**

- Automation hinzufügen (GitHub Actions)
- Erste 30-Tage Reviews durchführen
- Framework iterieren basierend auf Erfahrungen

**Rollback-Plan**: Bei signifikanten Problemen können wir auf informelle Entscheidungsfindung zurückfallen

## Alternativen betrachtet

### Alternative 1: Bestehende Prozesse beibehalten

**Beschreibung**: Kein formaler Rahmen, informelle Entscheidungen weiterhin

**Trade-offs**:

- Vorteile: Kein Overhead, maximale Geschwindigkeit
- Nachteile: Keine Nachvollziehbarkeit, schwer skalierbar, Lern-Verlust

**Warum abgelehnt**: Skalierungsprobleme und fehlende Transparenz würden mit Wachstum zu großen Problemen führen

### Alternative 2: Schweres Governance-Modell

**Beschreibung**: Formales Change-Management mit Komitees und Genehmigungen

**Trade-offs**:

- Vorteile: Maximale Kontrolle und Dokumentation
- Nachteile: Hoher Overhead, Innovations-Bremsung, gegen unsere Kultur

**Warum abgelehnt**: Würde gegen "Kontext > Kontrolle" und Speed-to-Learn Prinzipien verstoßen

### Alternative 3: Reiner OKR-Framework

**Beschreibung**: Objectives and Key Results für alle Entscheidungen

**Trade-offs**:

- Vorteile: Klare Metriken, Ausrichtung auf Ziele
- Nachteile: Zu rigid für kreative/explorative Entscheidungen, nicht für alle Entscheidungstypen geeignet

**Warum abgelehnt**: OKRs sind für strategische Ziele gut, aber nicht für operative/architekturelle Entscheidungen

## 30/90/365-Tage Impact

### 30 Tage

- Erste Entscheidungen mit Rahmen dokumentiert
- Team hat grundlegendes Verständnis
- Issue Templates werden aktiv genutzt
- Weniger "Warum diese Entscheidung?" Fragen

### 90 Tage

- Entscheidungsprozess läuft routiniert
- Erste Learnings aus 30-Tage Reviews
- Bessere Koordination zwischen Teams
- Transparenz für neue Teammitglieder

### 365 Tage

- Entscheidungen sind vollständig nachvollziehbar
- Organisationales Lernen beschleunigt
- Framework hat sich an Bedürfnisse angepasst
- Entscheidungsqualität signifikant verbessert

## Metriken & Erfolgsmessung

### Key Metrics

- **Adoption Rate**: % Entscheidungen, die Rahmen verwenden
- **Decision Velocity**: Zeit von Proposal bis Resolution
- **Learning Documentation**: % Entscheidungen mit dokumentierten Learnings
- **Team Satisfaction**: Feedback zu Entscheidungsprozess
- **Transparency Score**: % öffentlicher vs. vertraulicher Entscheidungen

### Review-Checkpoints

- **30-Tage-Review**: 2025-02-13 - Erste Nutzung und Feedback
- **90-Tage-Review**: 2025-04-13 - Prozess läuft routiniert
- **365-Tage-Review**: 2026-01-14 - Framework-Optimierung

## Implementierungs-Details

### Technische Spezifikationen

- GitHub Issues für Entscheidungsprozess
- ADR Markdown-Dateien für architekturelle Entscheidungen
- GitHub Actions für Automation
- Mermaid-Diagramme für Visualisierungen

### Dependencies

- GitHub Repository mit entsprechenden Berechtigungen
- Team buy-in für neue Prozesse
- Dokumentations-Standards

### Testing-Strategie

- Erste Entscheidungen als Piloten testen
- Framework iterativ verbessern
- A/B-Tests verschiedener Template-Versionen

## Offene Fragen

1. **Wie viel Overhead ist akzeptabel?** - Durch kontinuierliche Messung und Anpassung klären
2. **Wie fördern wir konsequente Nutzung?** - Automation und Kultur stärken
3. **Wie passen wir bei Wachstum an?** - Framework ist skalierbar designed

## Referenzen

- [Company Handbuch](../../profile/README.md) - Grundlegende Prinzipien
- [Entscheidungsrahmen](../DECISION_FRAMEWORK.md) - Detaillierte Dokumentation
- [Entscheidungsmatrix](../decision-matrix.md) - Praktische Anwendung
- [ADR Template](./template.md) - Für zukünftige ADRs

---

## Changelog

- 2025-01-14: ADR erstellt und als accepted markiert
- 2025-01-14: Framework-Implementierung gestartet
