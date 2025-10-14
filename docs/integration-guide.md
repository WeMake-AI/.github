# Integration Guide: Entscheidungsrahmen & Bestehende Praktiken

## Übersicht

Dieser Guide zeigt, wie der neue Entscheidungsrahmen mit bestehenden WeMake-Praktiken harmoniert und diese ergänzt. Der
Rahmen ist kein Ersatz, sondern eine Erweiterung unserer etablierten Prozesse.

## Bestehende Praktiken bei WeMake

### Company Handbuch (Kapitel 15)

- **PRs > Issues > Slack**: Entscheidungen und änderbare Vorschläge in PRs
- **Keine Issues an Personen zuweisen**: Teamorientierte Arbeit
- **Nicht einfach mergen ohne Review**: Mindestens ein Review für alle Änderungen
- **Dinge öffentlich machen**: Public by default

### RFCs (Request for Comments)

- Für technische und Produkt-Entscheidungen
- Strukturierte Diskussion vor Implementierung
- Öffentliche Kommentierung und Feedback

### Postmortems

- Nach Projektabschluss oder wichtigen Ereignissen
- Strukturiertes Lernen aus Erfolg und Misserfolg
- "Was haben wir gelernt?" statt "Wer war schuld?"

### Architektur-Entscheidungs-Records (ADRs)

- Für architekturell bedeutsame Entscheidungen
- Langlebige Dokumentation von Technologie-Entscheidungen
- Status-Tracking (proposed, accepted, deprecated)

## Integration des Entscheidungsrahmens

### 1. Ergänzung statt Ersatz

**Der Entscheidungsrahmen:**

- ✅ **Ergänzt** bestehende Prozesse durch strukturierte Entscheidungsfindung
- ✅ **Standardisiert** den Umgang mit verschiedenen Entscheidungstypen
- ❌ **Ersetzt NICHT** RFCs, Postmortems oder ADRs

**Beispiel-Integration:**

```
Entscheidungsvorschlag (Issue)
    ↓
RFC-Prozess (für technische Details)
    ↓
Entscheidungs-Record (Dokumentation)
    ↓
ADR (falls architekturell bedeutsam)
    ↓
PR-Implementierung (mit Entscheidungs-Link)
    ↓
Postmortem (nach 30/90/365 Tagen)
```

### 2. PRs & Issues Integration

#### Pull Request Template Enhancement

**Neue PR-Sections:**

- **Entscheidungsbezug**: Link zu Entscheidungs-Issue
- **Company Handbuch Checkliste**: Alignment-Prüfung
- **Alignment mit WeMake-Prinzipien**: Automatische Checks

**Bestehende PR-Praktiken bleiben:**

- Code Review durch Technical Leads
- Produkt Review durch Product Owner
- Dokumentations-Updates
- Testing-Anforderungen

#### Issue Template Integration

**Entscheidungsvorschlag Template:**

- Baut auf bestehenden Issue-Standards auf
- Fügt Entscheidungs-spezifische Felder hinzu
- Behält gewohnte GitHub-Issue-Struktur bei

**Entscheidungs-Record Template:**

- Für dokumentierte Entscheidungen
- Ergänzt bestehende Issue-Arbeitsweise
- Einfache Status-Verfolgung

### 3. RFC-Prozess Integration

#### Wann weiterhin RFCs verwenden?

**RFCs bleiben für:**

- Komplexe technische Architektur-Änderungen
- Produkt-Feature-Spezifikationen mit vielen Details
- Öffentliche Diskussionen vor Implementierung

**Entscheidungsrahmen + RFCs:**

1. **Entscheidungsvorschlag** erstellen (grobe Richtung)
2. **RFC** für technische Details und Spezifikationen
3. **Entscheidungs-Record** nach RFC-Abschluss
4. **ADR** falls architekturell bedeutsam

#### Beispiel: Feature-Entwicklung

```
1. Entscheidungsvorschlag: "Neues E-Mail-Feature für Clarity BI"
   - Problem: Kund:innen brauchen bessere E-Mail-Verarbeitung
   - Optionen: Eigenbau vs. Partner vs. Open-Source

2. RFC: "Technische Architektur für E-Mail-Processing"
   - API-Design, Datenmodelle, Integration-Details
   - Öffentliche Kommentierung und Feedback

3. Entscheidungs-Record: "E-Mail-Feature implementieren"
   - Finale Entscheidung nach RFC-Feedback
   - Umsetzungsplan und Metriken

4. ADR: Falls neue Architektur-Komponenten entstehen

5. PRs: Implementierung mit Links zu Entscheidungen
```

### 4. Postmortem Integration

#### Entscheidungs-Review als Postmortem-Ergänzung

**Entscheidungs-Framework Reviews:**

- **30-Tage-Review**: Erste Ergebnisse und Anpassungen
- **90-Tage-Review**: Muster und Trends erkennen
- **365-Tage-Review**: Langfristige Auswirkungen

**Bestehende Postmortems:**

- Nach Projektabschluss
- Nach wichtigen Ereignissen (Incidents, Launches)
- Strukturiertes Lernen aus Erfolg und Misserfolg

**Kombinierte Nutzung:**

```
Entscheidung getroffen
    ↓
Implementierung
    ↓
30-Tage-Entscheidungs-Review
    ↓
Projekt läuft weiter
    ↓
Projektabschluss-Postmortem
    ↓
90-Tage-Entscheidungs-Review
    ↓
365-Tage-Entscheidungs-Review
```

### 5. ADR-System Integration

#### Wann ADRs statt Entscheidungs-Issues?

**ADRs für:**

- **Architekturell bedeutsame** Type 1 Entscheidungen
- **Langlebige** Technologie-Entscheidungen
- **System-weite** Auswirkungen

**Entscheidungs-Issues für:**

- **Operative** Type 2 Entscheidungen
- **People & Culture** Entscheidungen
- **Nicht-architekturelle** strategische Entscheidungen

**Integration:**

```
Strategische Entscheidung (Issue)
    ↓
Ist sie architekturell bedeutsam?
    ├── JA → ADR erstellen
    └── NEIN → Issue-Record ausreichen

Operative Entscheidung (Issue)
    ↓
Braucht sie ADR?
    ├── JA → ADR zusätzlich zu Issue
    └── NEIN → Issue-Record
```

### 6. Company Handbuch Alignment

#### Wie der Rahmen Company Handbuch Prinzipien verkörpert

**Kapitel 11: "Du steuerst selbst"**

- Klare Entscheidungs-Owner (keine Committees)
- Kontext statt Kontrolle

**Kapitel 11: "Mach es öffentlich"**

- Public by default für alle Entscheidungen
- Transparenz als Qualitätsfilter

**Kapitel 11: "Warum nicht jetzt?"**

- Fast Decisions für reversible Type 2 Entscheidungen
- Bias für Action bei geringem Risiko

**Kapitel 15: "Keine Issues an Personen zuweisen"**

- Issues beschreiben Probleme
- Teams committen zu Lösungen
- Entscheidungs-Owner übernehmen Verantwortung

**Kapitel 15: "Nicht einfach mergen ohne Review"**

- Mindestens ein Review für alle Entscheidungen
- Entscheidungs-Alignment Check in PRs

## Praktische Beispiele

### Beispiel 1: Neue Produkt-Entscheidung

```
1. **Entscheidungsvorschlag Issue** erstellen
   - "Clarity BI um E-Mail-Processing erweitern"

2. **Stakeholder-Input** sammeln (async in Issue)

3. **RFC** für technische Spezifikationen

4. **Entscheidungs-Record** erstellen
   - Finale Entscheidung dokumentieren

5. **ADR** für neue Architektur-Komponenten

6. **PRs** für Implementierung
   - Mit Entscheidungs-Links

7. **30/90-Tage Reviews** als strukturierte Postmortems
```

### Beispiel 2: Operative Prozess-Änderung

```
1. **Entscheidungsvorschlag Issue** erstellen
   - "Async-First Kommunikation einführen"

2. **Schnelle Optionen** erkunden (Type 2)

3. **Entscheidungs-Record** erstellen

4. **PR** für Dokumentations-Änderungen

5. **30-Tage-Review** für erste Learnings
```

### Beispiel 3: Team-Kultur-Entscheidung

```
1. **Entscheidungsvorschlag Issue** erstellen
   - "Mentoring-Programm für Junior-Entwickler"

2. **Team-Input** sammeln

3. **Entscheidungs-Record** erstellen

4. **Keine ADR** (People & Culture, nicht architekturell)

5. **Implementierung** durch Richtlinien-Update

6. **90-Tage-Review** für Programm-Evaluation
```

## Migrations-Strategie

### Phase 1: Foundation (bereits abgeschlossen)

- ✅ Entscheidungsrahmen-Dokumentation erstellt
- ✅ ADR-System aufgesetzt
- ✅ Issue Templates implementiert
- ✅ GitHub Actions für Automation

### Phase 2: Team Adoption (aktuell)

- **Awareness schaffen**: Team über neuen Rahmen informieren
- **Erste Entscheidungen**: Pilot-Entscheidungen mit Rahmen
- **Feedback sammeln**: Anpassungen basierend auf Erfahrungen

### Phase 3: Optimization (nächste 30 Tage)

- **Automation erweitern**: Mehr GitHub Actions für Unterstützung
- **Prozess-Optimierung**: Rahmen an Team-Feedback anpassen
- **Integration vertiefen**: Bessere Verzahnung mit RFCs/Postmortems

## Erfolgsmessung

### Adoption-Metriken

- **Rahmen-Nutzung**: % Entscheidungen, die Rahmen verwenden
- **Template-Ausfüllung**: Vollständigkeit der Entscheidungs-Issues
- **Review-Durchführung**: % geplanter Reviews, die stattfinden

### Prozess-Metriken

- **Entscheidungs-Geschwindigkeit**: Zeit von Vorschlag bis Resolution
- **Entscheidungs-Qualität**: Retrospektive Bewertung durch Team
- **Lern-Effektivität**: Erkenntnisse aus Entscheidungs-Reviews

### Kultur-Metriken

- **Transparenz-Score**: % öffentlicher vs. vertraulicher Entscheidungen
- **Ownership-Klarheit**: % Entscheidungen mit klarem Owner
- **Lern-Kultur**: Häufigkeit von "Was haben wir gelernt?" Diskussionen

## Häufige Fragen & Antworten

### "Brauchen wir wirklich noch einen Rahmen?"

**Antwort:** Ja, aber er ist **pragmatisch** und **ergänzend**:

- Type 1: Vollständiger Prozess für wichtige Entscheidungen
- Type 2: Vereinfacht für reversible Experimente
- Integration mit bestehenden Praktiken

### "Wie unterscheidet sich das von RFCs?"

**RFCs:**

- Für technische Details und öffentliche Diskussion
- Nach Entscheidung für Spezifikation

**Entscheidungsrahmen:**

- Für die Entscheidungsfindung selbst
- Vor oder parallel zu RFCs
- Strukturiert den gesamten Prozess

### "Wann ist eine Entscheidung 'strategisch genug' für den vollen Prozess?"

**Rule of Thumb:**

- **Type 1**: Wenn Misserfolg signifikanten Schaden anrichtet
- **Type 2**: Wenn Misserfolg leicht reversibel ist
- **Entscheidungsmatrix** hilft bei der Klassifikation

### "Wie vermeiden wir Bürokratie?"

**Built-in Safeguards:**

- **Type 2** kann sehr schlank sein (15-Minuten-Entscheidungen)
- **Automation** reduziert manuellen Aufwand
- **Regelmäßige Reviews** stellen sicher, dass der Rahmen hilft statt hemmt

## Nächste Schritte

1. **Team-Workshop** planen (nächste Woche)
2. **Erste Pilot-Entscheidungen** mit Rahmen durchführen
3. **Feedback-Mechanismus** etablieren
4. **Kontinuierliche Verbesserung** des Frameworks

---

_Diese Integration entwickelt sich weiter. Der Entscheidungsrahmen soll helfen, nicht hindern. Bei Fragen oder
Verbesserungsvorschlägen: Issue öffnen._
