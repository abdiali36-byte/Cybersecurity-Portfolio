# Threat Intelligence

This section covers collecting, analysing, validating, and reporting threat intelligence relevant to SOC operations. Contents may include IOC research, OSINT investigations, MITRE ATT&CK mapping, and enrichment techniques used during triage and response.

# Threat Intelligence Report – [IOC, Threat Actor, or Campaign Name]

## Summary
Short description of the threat, IOC, or threat actor being investigated.

Example:
"Suspicious IP flagged via firewall logs and confirmed malicious through multiple reputation services."

---

## Scope of Investigation
| Type | Description |
|------|------------|
| IOC Lookup | Single IP, domain or hash |
| Threat Actor | Group profile |
| Campaign | Ongoing or historic |
| Other |  |

Tick one or add as needed.

---

## IOC / Indicator Details (If Applicable)

| Indicator Type | Value |
|----------------|-------|
| IP Address | |
| Domain | |
| File Hash | |
| URL | |

---

## OSINT and Reputation Results

| Source | Result | Notes |
|--------|--------|------|
| VirusTotal | |
| Talos | |
| AbuseIPDB | |
| Shodan | |
| Google Safe Browsing | |
| WhoIs Lookup | |

(Complete only those relevant)

---

## Threat Actor Profile (If Applicable)

| Field | Details |
|-------|--------|
| Threat Actor Name | |
| Suspected Region | |
| TTPs Used | |
| Known Targets | |
| Associated IOCs | |

---

## MITRE ATT&CK Mapping

| Tactic | Technique | Description |
|--------|----------|-------------|
| Initial Access | T1566 | Phishing |
| Credential Access | T1110 | Brute force |

(Add or remove rows as needed)

---

## Risk Assessment

| Impact Area | Level |
|-------------|-------|
| Reputation | |
| Data Confidentiality | |
| Operational Disruption | |
| Regulatory | |

---

## Recommended Defensive Actions
- Block IOC at firewall
- Add SIEM detection rule
- Update incident response playbook
- Inform third parties or internal stakeholders
- User awareness communication

---

## Narrative Summary (Manager Level)

Write this section as if explaining to a non-technical decision maker.

Example:
"This IOC is linked to credential harvesting campaigns targeting finance departments in UK businesses."

---

## Evidence

Attach:
- Screenshots (redacted)
- Query results
- Lookup exports
- Links

(Do not share confidential data)
