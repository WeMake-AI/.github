# Pull Request Template

## Beschreibung

**Was macht diese PR?** (Pflichtfeld)

<!-- Beschreibe kurz und präzise, was diese PR ändert oder hinzufügt -->

**Warum ist diese Änderung nötig?** (Pflichtfeld)

<!-- Erkläre das Problem oder die Opportunity, die diese PR adressiert -->

**Wie wurde das getestet?** (Pflichtfeld)

<!-- Beschreibe die Tests: Unit-Tests, Integration-Tests, manuelle Tests -->

## Entscheidungs-Kontext

### Ist diese PR Teil einer dokumentierten Entscheidung?

**Entscheidungsbezug:**

- [ ] Diese PR implementiert eine dokumentierte Entscheidung
- [ ] Diese PR ist unabhängig von größeren Entscheidungen

### Wenn Teil einer Entscheidung

**Entscheidungs-Issue:** #ISSUE_NUMMER

<!-- Link zum Entscheidungsvorschlag oder Entscheidungs-Record -->

**Entscheidungs-Owner:** @USERNAME

<!-- Person, die die Entscheidung getroffen hat -->

**Entscheidungs-Status:**

- [ ] proposed - Noch in Diskussion
- [ ] accepted - Entscheidung getroffen und wird umgesetzt
- [ ] rejected - Entscheidung wurde abgelehnt
- [ ] deprecated - Entscheidung wurde durch neuere ersetzt

## Alignment mit WeMake-Prinzipien

### Company Handbuch Checkliste

**Mission Alignment:**

- [ ] Trägt zur Transformation von Organisationen durch verantwortungsvolle KI bei?
- [ ] Fördert menschzentrierte KI-Entwicklung?

**Werte Alignment:**

- [ ] Unterstützt Transparenz und öffentliche Dokumentation?
- [ ] Fördert Ownership und Verantwortlichkeit?
- [ ] Ermöglicht Speed-to-Learn (schnelles Lernen)?

**Kulturelle Passung:**

- [ ] Folgt "Kontext > Kontrolle" Philosophie?
- [ ] Unterstützt "Klein anfangen, groß lernen"?
- [ ] Hält "Keine Perfektion erwarten" ein?

### Technische Standards

**Code Quality:**

- [ ] Code folgt bestehenden Patterns und Konventionen
- [ ] Tests sind ausreichend und passieren
- [ ] Dokumentation ist aktuell und hilfreich

**Security & Compliance:**

- [ ] DSGVO-Konformität sichergestellt (falls personenbezogene Daten)
- [ ] Security-Standards eingehalten
- [ ] Keine Hardcodierten Credentials oder sensiblen Daten

## Auswirkungen

### Was ändert sich für Nutzer:innen?

<!-- Beschreibe die Auswirkungen auf Endbenutzer:innen -->

### Was ändert sich für das Team?

<!-- Beschreibe die Auswirkungen auf interne Prozesse -->

### Was ändert sich für Kund:innen?

<!-- Beschreibe die Auswirkungen auf unsere Kund:innen -->

## Breaking Changes

### Gibt es Breaking Changes?

- [ ] Ja
- [ ] Nein

**Falls ja, beschreibe:**

<!-- Welche Änderungen brechen bestehende Integrationen oder Workflows? -->

**Migrations-Guide:**

<!-- Wie können Nutzer:innen/Kund:innen zu der neuen Version migrieren? -->

## Testing Checklist

### Vor Merge prüfen

**Funktionale Tests:**

- [ ] Neue Features funktionieren wie erwartet
- [ ] Bestehende Features wurden nicht beeinträchtigt
- [ ] Edge Cases wurden getestet

**Nicht-funktionale Tests:**

- [ ] Performance ist akzeptabel
- [ ] Security wurde geprüft
- [ ] Accessibility wurde berücksichtigt

**Dokumentation:**

- [ ] Code ist dokumentiert
- [ ] Öffentliche Dokumentation wurde aktualisiert
- [ ] Migrations-Guides sind verfügbar

## Review-Anforderungen

### Benötigte Reviewer

- **Code Review:** @USERNAME (Technische Korrektheit)
- **Produkt Review:** @USERNAME (Produkt-Alignment)
- **Dokumentation Review:** @USERNAME (Dokumentations-Updates)

### Review-Kriterien

- [ ] Code folgt Standards und ist wartbar
- [ ] Tests sind ausreichend und passieren
- [ ] Dokumentation ist klar und hilfreich
- [ ] Alignment mit Entscheidungen und Prinzipien

## Nach Merge

### Was passiert nach dem Merge?

**Automatische Schritte:**

- [ ] CI/CD Pipeline läuft automatisch
- [ ] Tests werden ausgeführt
- [ ] Deployment erfolgt (falls zutreffend)

**Manuelle Schritte:**

- [ ] Kund:innen informieren (falls Breaking Changes)
- [ ] Team intern kommunizieren
- [ ] Monitoring aktivieren

**Review-Plan:**

- [ ] 30-Tage-Review planen (für neue Features)
- [ ] Metriken definieren für Erfolgsmessung

## Zusätzliche Informationen

### Screenshots/Media

<!-- Falls relevant: Screenshots, Videos, oder andere Medien -->

### Verwandte Issues/PRs

<!-- Links zu verwandten Issues oder PRs -->

### Offene Fragen

<!-- Alles was noch geklärt werden muss -->

---

## WeMake PR Standards

Diese PR folgt den WeMake-Standards für:

- ✅ **Transparenz**: Alle Änderungen sind dokumentiert
- ✅ **Ownership**: Klare Verantwortlichkeit für die Änderung
- ✅ **Lernen**: Möglichkeit zum Lernen aus der Implementierung
- ✅ **Qualität**: Hohe Standards für Code und Dokumentation

**Erinnerung:** Bei Entscheidungs-PR immer die Entscheidungs-Issue verlinken und Alignment mit Company Handbuch
sicherstellen.
