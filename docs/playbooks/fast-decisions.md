# Fast Decisions Playbook

## Übersicht

Dieses Playbook hilft bei schnellen, reversiblen Entscheidungen - unserem "Warum nicht jetzt?"-Ansatz für Type 2
(Two-way door) Entscheidungen mit geringem Risiko und hoher Lern-Geschwindigkeit.

## Warum Fast Decisions?

### Company Handbuch Prinzipien

- **Warum nicht jetzt?** (Kapitel 11): Bias für Action bei reversiblen Entscheidungen
- **Klein anfangen, groß lernen** (Kapitel 11): Schnelle Experimente statt perfekter Pläne
- **Keine Perfektion erwarten** (Kapitel 15): Klar + funktionsfähig + dokumentiert

### Vorteile von Fast Decisions

- **Speed-to-Learn**: Schneller Feedback statt endloser Analyse
- **Geringes Risiko**: Leicht reversibel, begrenzter Impact
- **Team-Empowerment**: Schnelle Ownership statt Wartezeiten
- **Innovation fördern**: Niedrige Hürden für neue Ideen

## Wann Fast Decisions?

### Perfekte Kandidaten

- **Reversible Änderungen**: Können leicht zurückgenommen werden
- **Begrenzter Impact**: Weniger als 1 Woche Arbeit, unter 5k€ Kosten
- **Schneller Lern-Effekt**: Innerhalb von Tagen klar, ob es funktioniert
- **Niedriges Risiko**: Selbst bei Fehlschlag minimaler Schaden

### Nicht für Fast Decisions

- **Sicherheitsrelevante** Änderungen (DSGVO, Security)
- **Kund:innen-vertragliche** Verpflichtungen
- **Architekturell fundamentale** Entscheidungen
- **Finanzielle** Großentscheidungen (>10k€)

## Fast Decision Kategorien

### 15-Minuten-Entscheidungen

**Zeitrahmen**: 15 Minuten von Idee bis Entscheidung

**Beispiele:**

- **UI Tweaks**: Button-Farbe, Text-Änderung, Layout-Anpassung
- **Copy Changes**: Fehlermeldungen, Help-Text, Labels
- **Small Config**: Feature-Flags, A/B-Test Parameter
- **Documentation**: Kleine Updates, Link-Fixes, Tippfehler

**Prozess:**

1. **Problem identifizieren** (2 Min): Was stört mich/Kund:innen?
2. **Optionen brainstormen** (5 Min): 2-3 mögliche Lösungen
3. **Entscheiden** (3 Min): Welche Option testen wir?
4. **Umsetzen** (5 Min): Sofort machen oder Issue erstellen

### 1-Stunden-Entscheidungen

**Zeitrahmen**: Innerhalb einer Stunde

**Beispiele:**

- **Quick Fixes**: Bug-Workarounds, Hotfixes
- **Process Tweaks**: Meeting-Format, Tool-Konfiguration
- **Content Updates**: Blog-Post, Dokumentations-Änderung
- **Team Coordination**: Standup-Format, Retro-Struktur

**Prozess:**

1. **Kontext teilen** (10 Min): Betroffene informieren
2. **Optionen diskutieren** (20 Min): Schnelle Abwägung
3. **Entscheidung treffen** (10 Min): Klarer Owner, klare Richtung
4. **Umsetzen planen** (20 Min): Nächste Schritte definieren

### 1-Tages-Entscheidungen

**Zeitrahmen**: Innerhalb eines Arbeitstages

**Beispiele:**

- **Feature Experiments**: Neue Funktionalität testen
- **Process Changes**: Workflow-Optimierung
- **Tool Evaluation**: Neues Tool/Plugin testen
- **Team Structure**: Kleine Anpassungen

**Prozess:**

1. **Morgen**: Problem analysieren, erste Recherche
2. **Mittag**: Optionen entwickeln, Stakeholder informieren
3. **Abend**: Entscheidung treffen und kommunizieren

## Fast Decision Prozess

### 1. Kontext sammeln (minimal)

**Was brauchen wir?**

- **Problem klar definieren**: Was ist das eigentliche Issue?
- **Betroffene identifizieren**: Wer muss wissen/betroffen?
- **Erfolgs-Kriterien**: Wie wissen wir, dass es funktioniert?

**Company Handbuch Check:**

- **Wirkung** (Kapitel 5): Löst es echte Probleme für Nutzer:innen?
- **Lernen** (Kapitel 11): Was können wir daraus lernen?

### 2. Optionen erkunden (pragmatisch)

**Mindestens 2-3 Optionen:**

- **Status Quo**: Was passiert wenn wir nichts ändern?
- **Quick Fix**: Minimaler Aufwand für sofortige Verbesserung
- **Proper Solution**: Nachhaltiger, aber aufwändiger

**Trade-off Betrachtung:**

- **Aufwand**: Wie viel Zeit/Ressourcen?
- **Impact**: Wie viel Verbesserung erwarten wir?
- **Risiko**: Was ist das Worst-Case-Szenario?

### 3. Impact-Analyse (vereinfacht)

**30-Tage-Fokus:**

- **Sofortige Auswirkung**: Was ändert sich nächste Woche?
- **Erste Metriken**: Welche Zahlen werden sich bewegen?
- **Feedback-Loop**: Wie bekommen wir schnell Rückmeldung?

**Keine ausführliche 90/365-Analyse für Fast Decisions** - das lernen wir durch das Experiment.

### 4. Entscheidung treffen (sofort)

**Entscheidungs-Owner:** Person mit dem besten Kontext oder der meisten Erfahrung

**Entscheidungskriterien:**

1. **Schnelligkeit**: Wie schnell können wir lernen?
2. **Reversibilität**: Können wir zurückrudern?
3. **Lern-Potential**: Was erfahren wir Neues?
4. **Risiko-Level**: Akzeptables Downside-Risiko?

### 5. Learning & Iteration (aggressiv)

**Schnelle Feedback-Loops:**

- **Täglich**: Erste Beobachtungen tracken
- **Wöchentlich**: Strukturierte Review
- **Monatlich**: Entscheidung anpassen oder stoppen

**Exit-Kriterien definieren:**

- **Wann stoppen?** Klare Kriterien für "Das funktioniert nicht"
- **Wann skalieren?** Erfolgs-Kriterien für "Mehr davon machen"

## Fast Decision Templates

### 15-Minuten-Decision Record

```
**Entscheidung:** [Was haben wir entschieden?]
**Problem:** [Warum haben wir das entschieden?]
**Optionen:**
- Option 1: [Kurze Beschreibung]
- Option 2: [Kurze Beschreibung]
**Entscheidung:** [Welche Option + warum]
**Erfolgs-Kriterien:** [Wie messen wir Erfolg?]
**Review:** [Wann schauen wir nochmal hin?]
```

### 1-Stunden-Decision Issue

```yaml
# Entscheidung: [Titel]

## Problem
[Kurze Problem-Beschreibung]

## Optionen
- **Option 1:** [Beschreibung + Trade-offs]
- **Option 2:** [Beschreibung + Trade-offs]
- **Option 3:** [Beschreibung + Trade-offs]

## Entscheidung
[Gewählte Option + Rationale]

## Umsetzung
[Was passiert als nächstes?]

## Erfolgsmessung
[Metriken + Zeitpunkte]

## Review
[30-Tage-Checkpoint]
```

## Kommunikation bei Fast Decisions

### Wen informieren?

**Always:**

- **Direkt Betroffene**: Teammitglieder, die die Änderung umsetzen
- **Stakeholder**: Personen, deren Arbeit sich ändert

**Sometimes:**

- **Leadership**: Bei breiteren Auswirkungen
- **Kund:innen**: Bei Nutzererfahrungs-Änderungen

**Never (für Fast Decisions):**

- **All-Hands**: Zu kleinteilig für volle Aufmerksamkeit
- **Newsletter**: Operative Details interessieren nicht alle

### Wie kommunizieren?

**Für 15-Minuten-Entscheidungen:**

- GitHub Issue erstellen
- Betroffene per Slack/Teams mentionen
- Issue-Link teilen

**Für 1-Stunden-Entscheidungen:**

- Issue erstellen und diskutieren
- Async-Feedback sammeln
- Entscheidung dokumentieren

**Für 1-Tages-Entscheidungen:**

- Morgen: Issue erstellen, Kontext teilen
- Mittag: Optionen diskutieren
- Abend: Entscheidung kommunizieren

## Häufige Fast Decision Patterns

### UI/UX Tweaks

**Beispiel:** Button-Text ändern von "Senden" zu "Absenden"

**Prozess:**

1. Problem: "Senden" ist zu generisch, "Absenden" klarer für deutsche Nutzer:innen
2. Optionen: "Senden", "Absenden", "Übermitteln"
3. Entscheidung: "Absenden" - besserer Kontext
4. Umsetzung: Code-Änderung in 5 Minuten
5. Review: A/B-Test nach 1 Woche

### Process Improvements

**Beispiel:** Standup-Format ändern

**Prozess:**

1. Problem: Aktuelle Standups dauern 45 Minuten, bringen wenig Wert
2. Optionen: Abschaffen, Kürzen auf 15 Minuten, Async-Format
3. Entscheidung: 15-Minuten-Format testen
4. Umsetzung: Neue Struktur kommunizieren
5. Review: Nach 2 Wochen evaluieren

### Tool Changes

**Beispiel:** Neues Monitoring-Tool testen

**Prozess:**

1. Problem: Aktuelles Monitoring zu komplex, Team nutzt es nicht
2. Optionen: Bestehendes optimieren, Einfacheres Tool finden
3. Entscheidung: Einfacheres Tool testen (kostenloser Trial)
4. Umsetzung: Tool installieren, Team schulen
5. Review: Nach 30 Tagen entscheiden ob behalten

## Risiko-Management für Fast Decisions

### Akzeptable Risiken

- **Zeit-Investition**: 1-5 Tage Arbeit
- **Kosten**: Unter 1.000€
- **Opportunity Cost**: Andere Dinge bleiben liegen
- **Team-Frustration**: Wenn es nicht funktioniert

### Nicht akzeptable Risiken

- **Sicherheitsprobleme**: DSGVO-Verstöße, Data Leaks
- **Kund:innen-Schaden**: Vertragsbruch, Service-Unterbrechungen
- **Team-Schaden**: Überlastung, Burnout
- **Reputationsschaden**: Öffentliche Probleme

### Risiko-Mitigation

1. **Kleine Batches**: Nicht alles auf einmal ändern
2. **Feature Flags**: Änderungen abschaltbar machen
3. **Rollback-Plan**: Wie machen wir es rückgängig?
4. **Stakeholder informieren**: Überraschungen vermeiden

## Erfolgs-Beispiele

### Gute Fast Decisions bei WeMake

- **Async-First Kommunikation**: Von täglichen Meetings zu dokumentenbasierten Updates
- **Issue-First Development**: Alle Entscheidungen in GitHub statt in Slack
- **MVP-Features**: Schnelle Prototypen statt perfekter Features

### Schlechte Fast Decisions (und was wir gelernt haben)

- **Tool-Wechsel ohne Migration**: Daten verloren, Team frustriert
  - **Lektion**: Rollback-Plan ist Pflicht
- **Prozess-Änderung ohne Kommunikation**: Team war überrascht
  - **Lektion**: Betroffene immer informieren

## Tools für Fast Decisions

### Einfache Tools

- **GitHub Issues**: Für Dokumentation und Tracking
- **Google Docs/Sheets**: Für schnelle Analysen
- **Figma/Miro**: Für Visualisierungen
- **Slack/Teams**: Für schnelle Abstimmungen

### WeMake-spezifische Tools

- **Clarity BI**: Für Daten-gestützte Entscheidungen
- **V41 Platform**: Für operative Workflows
- **GitHub Templates**: Für standardisierte Dokumentation

## Kontinuierliche Verbesserung

### Metrics für Fast Decisions

- **Decision Velocity**: Wie schnell von Idee zu Umsetzung?
- **Success Rate**: Wie viele Fast Decisions erreichen ihre Ziele?
- **Learning Speed**: Wie schnell passen wir basierend auf Feedback an?
- **Team Satisfaction**: Wie fühlt sich das Team bei diesem Prozess?

### Regelmäßige Reviews

- **Wöchentlich**: Was können wir bei Fast Decisions besser machen?
- **Monatlich**: Patterns erkennen und optimieren
- **Quartalsweise**: Framework anpassen

---

_Fast Decisions sind der Motor unserer Speed-to-Learn Kultur. Sie ermöglichen es uns, schnell zu lernen und
kontinuierlich zu verbessern._
