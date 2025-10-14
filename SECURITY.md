# WeMake Sicherheitsrichtlinie

## Enterprise-Sicherheitsstandards

WeMake unterhält Enterprise-Grade-Sicherheitsstandards für alle Implementierungen von Model Context Protocol
(MCP)-Servern, KI-Agenten-Integrationen einschließlich Clarity BI (meetclarity.de / clarity.bi) sowie Cloudflare
Workers-Deployments. Unser Sicherheitsframework ist darauf ausgelegt, deutsche und europäische Regulierungsanforderungen
zu erfüllen, einschließlich DSGVO (GDPR), NIS2 und aufkommender KI-Governance-Standards.

## Unterstützte Versionen

Wir finalisieren derzeit unsere formale Support-Policy. Zwischenzeitliche Verpflichtung:

- Unterstützte Versionen: neueste zwei Minor-Releases von 1.x (rollendes Fenster)
- Sicherheitsupdates: Critical/High für unterstützte Versionen
- EOL (End-of-Life): 90 Tage nach dem nächsten Minor-Release
- Vollständige Policy wird bis Ende 2025 veröffentlicht. Tracking: <https://github.com/wemake-ai/mcp/issues/32>

Diese Sicherheitsrichtlinie wurde zuletzt im August 2025 aktualisiert und gilt für betroffene Personen im Europäischen
Wirtschaftsraum und der Schweiz.

## KI-Sicherheitsframework

### Model Context Protocol (MCP) Security

- **Authentifizierung & Autorisierung**: Mehrschichtige Zugriffskontrollen mit rollenbasierten Berechtigungen für
  MCP-Server-Interaktionen
- **Datenvalidierung**: Strikte Input/Output-Validierung für alle MCP-Tool-Aufrufe und -Antworten, einschließlich
  E-Mail-Inhalten und Dokumentenverarbeitung
- **Code-Verständnis & Review**: Priorisierung der Sicherheit durch umfassende Code-Review-Prozesse, da das Verstehen
  von Code kritischer ist als dessen Generierung. Implementierung obligatorischer menschlicher Überprüfung für
  KI-generierten sicherheitskritischen Code
- **SAST/DAST/SCA**: Statische/dynamische Analysen und Dependency-Audits obligatorisch in CI
- **SBOM**: Signierte SBOMs (z. B. SPDX/CycloneDX) für MCP-Server und KI-Agenten
- **Test-Coverage-Gate**: ≥90 % (Branches/Lines) als Merge-Anforderung für sicherheitsrelevante Komponenten
- **Sandboxing**: Isolierte Ausführungsumgebungen für KI-Agenten-Operationen, einschließlich sicherer E-Mail- und
  Dokumentenverarbeitung
- **Audit-Logging**: Umfassendes Logging aller KI-Interaktionen für Compliance- und Sicherheitsmonitoring
- **Rate Limiting**: Erweiterte Drosselungsmechanismen zur Missbrauchsprävention und Sicherstellung der
  Service-Verfügbarkeit
- **Content Security**: Dateityp-Validierung, Malware-Scanning und sichere Verarbeitung von Anhängen für E-Mail- und
  Dokumenten-Inputs

### Cloudflare Workers Security

- **Edge Security**: Nutzung der globalen Sicherheitsinfrastruktur von Cloudflare
- **Zero Trust Architecture (Edge/Access)**: Kein implizites Vertrauen für Komponenten oder Benutzer
- **DDoS Protection**: Integrierter Schutz gegen Distributed-Denial-of-Service-Angriffe
- **Encryption in Transit (TLS)**: TLS 1.2+/1.3; mTLS für Service-to-Service-Traffic (Details siehe
  [Datenschutz & Verschlüsselung](#datenschutz--verschlüsselung))
- **Content Security Policy**: Strikte CSP-Header zur Abwehr von XSS- und Injection-Angriffsvektoren

### DSGVO & Datenschutz

- **Datenminimierung**: Erhebung ausschließlich notwendiger Daten für KI-Operationen, einschließlich E-Mail- und
  Dokumentenverarbeitung
- **Zweckbindung**: Verwendung von Daten ausschließlich für spezifizierte, legitime Zwecke
- **Speicherbegrenzung**: Automatisierte Datenaufbewahrungs- und Löschrichtlinien mit gestaffelten Speicheransätzen
- **Betroffenenrechte**: Umfassende Unterstützung für Auskunfts-, Berichtigungs- und Löschungsanträge
- **Privacy by Design**: Eingebaute Datenschutzmaßnahmen in allen KI-Systemen
- **Grenzüberschreitende Übermittlungen**: Konforme Datentransfermechanismen für globale Operationen
- **Datenübertragbarkeit/Einschränkung/Widerspruch**: Unterstützung für Anfragen gemäß Art. 20/18/21 DSGVO
- **DSFA**: Datenschutz-Folgenabschätzungen für Hochrisiko-Verarbeitungen (Art. 35 DSGVO)
- **VVT**: Verzeichnis von Verarbeitungstätigkeiten wird geführt (Art. 30 DSGVO)
- **Benutzerdatenexport und -löschung**: Sichere Exportfunktionen und automatisierte Löschung für Benutzerdaten und
  verarbeitete Inhalte
- **Einreichung von DSR (Data Subject Requests)**: [privacy@wemake.cx](mailto:privacy@wemake.cx) oder DSR-Portal:
  [https://wemake.cx/privacy/requests](https://wemake.cx/privacy/requests)

## Schwachstellen-Meldung

### Verantwortungsvolle Offenlegung (Responsible Disclosure)

Wir fördern die verantwortungsvolle Offenlegung von Sicherheitsschwachstellen. Bitte melden Sie Sicherheitsprobleme an:

**E-Mail**: [security@wemake.cx](mailto:security@wemake.cx)  
**PGP-Schlüssel**: [Öffentlichen Schlüssel herunterladen](https://wemake.cx/.well-known/pgp-key.asc)  
**PGP-Fingerprint**: `3DAA 7730 D3FB B35D D9B9 1E2C 3BF4 9577 F25A 95D5`  
**Antwortzeit**: Erste Bestätigung innerhalb von 24 Stunden  
**PGP-Key-ID**: 3BF49577F25A95D5  
**Algorithmus**: ed25519  
**Gültig bis**: 2027-08-17 (Rotationsrichtlinie: halbjährlich)

#### Safe-Harbor-Regelung

WeMake unterstützt gutgläubige Sicherheitsforschung. Wenn Sie dieser Richtlinie entsprechen und verantwortungsvoll
handeln, werden wir keine rechtlichen Schritte gegen Ihre Forschungsaktivitäten einleiten.

#### security.txt

Unsere Sicherheitsoffenlegungsdetails sind ebenfalls veröffentlicht unter:  
[security.txt (RFC 9116)](https://wemake.cx/.well-known/security.txt)

### Meldungsrichtlinien

Bei der Meldung von Schwachstellen fügen Sie bitte folgende Informationen bei:

1. **Schwachstellentyp**: Klassifizierung (z. B. KI-Sicherheit, Datenschutz, Infrastruktur)
2. **Betroffene Komponenten**: Spezifische MCP-Server, KI-Agenten oder Infrastrukturkomponenten
3. **Impact-Assessment**: Potenzielle geschäftliche und sicherheitstechnische Auswirkungen
4. **Reproduktionsschritte**: Detaillierte Schritte zur Reproduktion der Schwachstelle
5. **Proof of Concept**: Nicht-destruktive Demonstration, falls anwendbar
6. **Vorgeschlagene Remediation**: Vorgeschlagene Fixes oder Mitigationsmaßnahmen

### Sicherheits-Response-Prozess

1. **Bestätigung** (24h): Empfangsbestätigung und initiales Triage
2. **Untersuchung** (72h): Technische Analyse und Impact-Assessment
3. **Schweregrad-Klassifizierung**: CVSS v3.1 Score-Mapping zu Critical/High/Medium/Low
4. **Remediation** (Ziel-SLAs): Critical ≤7d, High ≤14d, Medium ≤30d, Low ≤90d (best effort)
5. **Offenlegung** (30–90d): Koordinierte öffentliche Offenlegung nach Remediation
6. **Anerkennung**: Öffentliche Würdigung verantwortungsvoller Melder (mit Einwilligung)

Hinweise zu Zeitangaben:

- SLAs beziehen sich auf Kalendertage, sofern nicht anders angegeben; Zeitzone: UTC
- Koordinierte Offenlegungs- und Embargo-Perioden werden wie vereinbart eingehalten
- SLA-Start: bei Eingang bei [security@wemake.cx](mailto:security@wemake.cx) (Mailserver-Zeitstempel)
- CVE-Handhabung: Wir beantragen CVEs (über CNA oder MITRE) für qualifizierende Issues und koordinieren IDs vor
  Offenlegung

#### CVSS v3.1 Mapping (Leitfaden)

- None: 0,0
- Critical: 9,0–10,0
- High: 7,0–8,9
- Medium: 4,0–6,9
- Low: 0,1–3,9

## Technische und organisatorische Maßnahmen

### Enterprise-KI-Sicherheitskontrollen

WeMake hat umfassende technische und organisatorische Maßnahmen implementiert, die für Enterprise-KI-Entwicklung und
MCP-Server-Operationen angemessen sind:

#### Datenschutz & Verschlüsselung

- **Verschlüsselung im Ruhezustand & bei Übertragung**: AES-256-Verschlüsselung für Daten im Ruhezustand; TLS 1.2+/1.3
  mit starken Cipher Suites (AES-GCM-256 oder ChaCha20-Poly1305) für Daten bei Übertragung, einschließlich
  E-Mail-Inhalten und Dokumentenverarbeitung
- **Key Management**: Hardware Security Modules (HSMs) für kryptografischen Schlüsselschutz
- **Pseudonymisierung/Anonymisierung**: Pseudonymisierung standardmäßig; Anonymisierung wo durchführbar für
  KI-Trainingsdaten
- **Data Masking**: Dynamisches Data Masking für Entwicklungs- und Testumgebungen
- **Content-Processing-Security**: Ende-zu-Ende-Verschlüsselung für E-Mail- und Dokumenteninhalte während Verarbeitung
  und Speicherung

#### KI-Systemsicherheit

- **Modellintegrität**: Kryptografische Signaturen zur Verifikation von KI-Modellen
- **Prompt-Injection-Schutz**: Erweiterte Filterung und Validierung für KI-Inputs
- **Output-Sanitization**: Umfassende Validierung von KI-generierten Inhalten
- **Adversarial Defense**: Schutz gegen Model Poisoning und Evasion-Angriffe
- **Model Supply Chain Security**: Signierte Artefakte (z. B. Sigstore), SLSA-Level-Ziele und Provenance-Attestierungen
- **Model/Dataset Cards**: Standardisierte Dokumentation zu Provenienz, Verwendungszweck, Limitationen und Risiken

#### Infrastruktursicherheit

- **Zero Trust Network**: Mikrosegmentierung und kontinuierliche Verifikation
- **Container Security**: Gehärtete Container-Images mit Schwachstellen-Scanning
- **Secrets Management**: Automatisierte Rotation und sichere Speicherung von Credentials
- **Netzwerkisolation**: Segregierte Umgebungen für verschiedene Sicherheitszonen
- **Egress Filtering**: Restriktive Outbound-Firewall-Policies; Erlaubnis nur für erforderliche Ziele/Ports
- **DNS Security**: DNSSEC/DoT/DoH, Threat-Intelligence-Blocklists und Egress-DNS-Pinning

#### Operative Sicherheit

- **Continuous Monitoring**: 24/7-Security-Operations-Center (SOC)-Monitoring
- **Incident Response**: Automatisierte Threat-Detection- und Response-Fähigkeiten
- **Backup & Recovery**: Automatisierte, verschlüsselte Backups mit getesteten Wiederherstellungsverfahren
- **Business Continuity**: Disaster-Recovery-Pläne mit definierten RTO/RPO-Zielen

#### Compliance & Governance

- **Regelmäßige Audits**: Vierteljährliche Sicherheitsbewertungen und Penetrationstests
- **Compliance-Monitoring**: Automatisierte DSGVO- und Regulierungs-Compliance-Prüfung
- **Risikobewertung**: Kontinuierliche Risikoevaluierung und Mitigationsstrategien
- **Sicherheitsschulungen**: Regelmäßige Security-Awareness-Schulungen für alle Mitarbeitenden

### KI-spezifische Risikominderung

Unser Sicherheitsframework adressiert einzigartige Risiken in der KI-Entwicklung und erkennt an, dass Code-Verständnis
die primäre Sicherheitsherausforderung darstellt:

- **Code-Comprehension-Security**: Obligatorische Dokumentation zur Erklärung von KI-generierten Code-Entscheidungen und
  Sicherheitsimplikationen
- **Review-Quality-Assurance**: Erweiterte Review-Prozesse für KI-generierten Code mit Fokus auf Verständnis über
  Geschwindigkeit
- **Data Poisoning**: Robuste Datenvalidierung und Provenance-Tracking
- **Model Extraction**: Schutz gegen unauthorisierten Modellzugriff und Replikation
- **Bias Detection**: Automatisiertes Monitoring für algorithmische Verzerrungen und Fairness
- **Explainability**: Transparente KI-Entscheidungsprozesse für Audit-Trails mit Schwerpunkt auf Reviewer-Verständnis
- **Human Oversight**: Obligatorische menschliche Überprüfung für Hochrisiko-KI-Entscheidungen mit ausreichender Zeit
  für angemessenes Verständnis

---

_Diese Sicherheitsrichtlinie wird regelmäßig aktualisiert, um aufkommende Bedrohungen in KI und Enterprise-Security zu
adressieren. Zuletzt aktualisiert: August 2025_

## Kontakt & Support

Für sicherheitsbezogene Anfragen, Schwachstellenmeldungen oder Compliance-Fragen zu allen WeMake-Produkten
einschließlich Clarity BI:

- **Security Team**: [security@wemake.cx](mailto:security@wemake.cx)
- **Emergency Hotline**: 24/7 verfügbar für kritische Sicherheitsvorfälle

WeMake verpflichtet sich zur Aufrechterhaltung höchster Standards für Sicherheit und Datenschutz in allen
KI-Entwicklungs- und Deployment-Aktivitäten, einschließlich E-Mail- und Dokumentenverarbeitungssystemen.
