Incident Reports

This section contains cybersecurity incident response reports based on simulated or real-world styled scenarios. Each report follows a standard IR structure: preparation, identification, containment, eradication, recovery, and lessons learned.

These reports demonstrate analytical thinking, defensive response strategy, and the ability to communicate technical findings clearly to both technical and non-technical stakeholders.
# Incident Report – [Title of Incident]

## Summary
Short overview of the incident, how it was detected, and the current status.

Example:
"Phishing email reported by employee resulted in unauthorized access attempt."

---

## Timeline of Events
| Date/Time (UTC) | Event Description | Source |
|----------------|------------------|-------|
| 12:43 | Alert triggered | Defender for 365 |
| 12:45 | SOC analyst review begins | Analyst |
| 12:47 | User contacted | HR |

---

## 1. Preparation
What controls, policies, or tools existed before the incident?
- Email filtering
- MFA enforcement
- Security awareness training
- Logging/monitoring

---

## 2. Detection and Analysis
- How was the incident detected?
- What tools triggered the alert?
- What data sources were used to analyze it?

Example data sources:
- SIEM logs
- Email header analysis
- AV / EDR alert
- Entra ID sign-in log
- User report

**Root Cause Analysis**
Why did it happen?

---

## 3. Containment, Eradication & Recovery

### Containment
Actions taken to stop the threat.

| Action | Responsible | Status |
|--------|------------|-------|
| Block sender | SOC | Done |
| Disable account | IAM | Done |

### Eradication
Actions taken to remove the threat.

### Recovery
Actions taken to restore normal operations.

---

## 4. Post-Incident Activity (Lessons Learned)
- What worked well?
- What delayed response?
- What should change?

**Preventive Controls Suggested**
- Policy improvement
- Training
- Technical hardening

---

## MITRE ATT&CK Mapping (If Applicable)
| Tactic | Technique |
|--------|----------|
| Phishing | T1566 |
| Valid Accounts | T1078 |

---

## Evidence
Attach screenshots, logs, reports (redacted).
Do NOT upload confidential data.
