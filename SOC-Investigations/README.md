Notes and investigations from SOC-style labs and SIEM exercises

# SOC Investigation – [Alert Name or Case Title]

## Summary
High-level explanation of the alert and reason for investigation.
(Write this as if explaining to a manager, not an engineer.)

Example:
"A login alert was triggered from an unusual geographic region, requiring validation to determine whether it was legitimate or a potential account compromise."

---

## Alert Details
| Field | Value |
|------|-------|
| Alert Name |  |
| Severity |  |
| Source System |  |
| Time Observed |  |
| Asset/User |  |

---

## Investigation Questions
Key questions you are trying to answer:

- Is this activity expected?
- Is the user valid or compromised?
- Is the device known or unknown?
- Does behaviour match business activity?
- Does this require escalation?

---

## Data Sources Reviewed
(Select or delete)

- Cloud identity logs
- Endpoint security alerts
- Firewall or web proxy logs
- Email security logs
- DNS logs
- Threat intelligence feeds
- OSINT lookups

---

## Technical Investigation Steps
(Number and document your steps clearly.)

1. Searched for event ID or signature in SIEM  
2. Filtered logs related to IP, user or device  
3. Checked previous behaviour from same entity  
4. Performed IP/Domain reputation lookup  
5. Validated timestamp and geo-location  

---

## Findings (Technical + Narrative)

**Technical Findings**
- What the logs show
- Patterns observed
- Any anomalies

**Non-Technical Summary**
Explain clearly why this matters.

Example:
"This behaviour is unlikely to be legitimate because the user was active in the UK five minutes earlier."

---

## Risk Assessment
Example fields:

| Category | Impact |
|----------|--------|
| Data Exposure | Medium |
| Account Takeover | High |
| Privilege Escalation | Low |

---

## Recommended Actions
| Action | Priority | Owner | Status |
|--------|---------|--------|-------|
| Force password reset | High | IAM |
| Block IP | Medium | Network |
| Enable MFA | High | Security |
| Educate user | Low | HR/Training |

---

## Escalation Decision
- Closed as false positive
- Escalated to Incident Response
- Monitoring only
- Awaiting additional data

(Add notes)

---

## MITRE ATT&CK Mapping
| Tactic | Technique |
|--------|----------|
| Initial Access | Phishing |
| Credential Access | Valid Accounts |
| Persistence | Account manipulation |

---

## Evidence
- Screenshots (redacted)
- Log snippets
- Query examples
