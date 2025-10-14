# Architecture Decision Records (ADRs)

## Übersicht

Architecture Decision Records (ADRs) dokumentieren die architekturell bedeutsamen Entscheidungen in WeMake. Sie folgen
dem [ADR-Format](https://adr.github.io/) und sind ein wichtiger Bestandteil unseres Entscheidungsrahmens.

## Warum ADRs?

ADRs helfen uns bei:

- **Nachvollziehbarkeit**: Architektur-Entscheidungen sind für alle einsehbar
- **Lernen**: Aus vergangenen Entscheidungen lernen
- **Konsistenz**: Einheitliche Dokumentation von Technologie-Entscheidungen
- **Kommunikation**: Stakeholder verstehen die Rationale hinter Entscheidungen

## Wann ADRs verwenden?

ADRs sind für **Type 1 Entscheidungen** mit architektureller Bedeutung obligatorisch:

### Architekturell bedeutsame Entscheidungen

- Technologie-Stack-Änderungen
- System-Architektur-Entscheidungen
- Datenmodell-Änderungen
- Sicherheitsrelevante Architektur-Entscheidungen
- Plattform-übergreifende Integrationen

### Nicht für ADRs geeignet

- Feature-spezifische Implementierungsdetails
- UI/UX-Design-Entscheidungen (außer architekturell relevant)
- Operative Prozess-Änderungen
- People & Culture Entscheidungen

## ADR-Nummerierung

ADRs werden fortlaufend nummeriert:

- `0001-decision-framework.md` - Meta-ADR für den Entscheidungsrahmen selbst
- `0002-*` - Erste echte Architektur-Entscheidung
- Fortlaufende Nummerierung für alle zukünftigen ADRs

## ADR-Status

Jedes ADR hat einen Status:

- **proposed** - Vorschlag in Diskussion
- **accepted** - Entscheidung getroffen und umgesetzt
- **deprecated** - Entscheidung wurde durch neuere ersetzt
- **superseded** - Entscheidung wurde aufgehoben

## Template verwenden

Verwende das [ADR Template](./template.md) für neue Entscheidungen.

## Verzeichnisstruktur

```
docs/decisions/
├── README.md (dieses Dokument)
├── template.md (ADR-Template)
├── 0001-decision-framework.md (Meta-ADR)
├── 0002-example-architecture.md
└── ...
```

## Integration mit Entscheidungsrahmen

ADRs sind Teil unseres 5-Stufen-Entscheidungsprozesses:

1. **Kontext**: Problem und Architektur-Kontext beschreiben
2. **Optionen**: Architekturale Alternativen evaluieren
3. **Impact**: Architekturelle Auswirkungen analysieren
4. **Entscheidung**: ADR als Entscheidungs-Record
5. **Learning**: ADR-Status und Lessons Learned aktualisieren

## Links zu anderen Dokumenten

- [Entscheidungsrahmen](../DECISION_FRAMEWORK.md) - Übergeordneter Rahmen
- [Entscheidungsmatrix](../decision-matrix.md) - Template-Auswahlhilfe
- [Company Handbuch](../../profile/README.md) - Unternehmensprinzipien

---

_ADRs entwickeln sich mit unserer Architektur weiter. Bei Fragen: Issue öffnen oder PR erstellen._
