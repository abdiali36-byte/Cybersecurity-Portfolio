 Cloud Security (Defensive)

This section focuses on defensive cloud security concepts, investigations, and configurations with a focus on Microsoft cloud environments (Entra ID, Azure AD, Microsoft 365, and Sentinel).

Topics and projects in this section will include:

- Conditional Access policies
- MFA enforcement and bypass investigation
- Entra ID sign-in log analysis
- Impossible travel alerts
- Privileged role misuse
- Email and Teams phishing workflows (Defender for 365)
- Tenant hardening recommendations

The goal is to demonstrate practical defensive capability and investigation skills in cloud-first environments that align with modern SOC operations.

# Cloud Security Case Study – [Title of Issue or Investigation]

## Summary
Brief description of the cloud security issue, misconfiguration, or investigation being performed.

Example:
"Investigating impossible travel sign-in alerts triggered from two geographic locations within minutes."

---

## Objective
What are you trying to prove, resolve, or understand?

- Determine if the alert represents genuine compromise or false positive.
- Validate MFA, Conditional Access or identity protection configuration.
- Identify potential gaps in cloud tenant security.

---

## Tools & Data Sources Used
- Microsoft Entra ID / Azure AD sign-in logs
- Conditional Access policy audit
- Defender for 365 alerts
- Sentinel queries (if used)
- API lookups, if enrichment applied

---

## Investigation Steps
Document the step-by-step process:

1. Reviewed sign-in logs for originating IPs  
2. Checked MFA requirement enforcement  
3. Compared against user travel history  
4. Validated ISP geolocation  
5. Reviewed Conditional Access outcomes  

---

## Findings
Summarise what the investigation revealed.

Example:
- Sign-in originated from VPN exit node
- MFA was bypassed due to legacy protocol
- Conditional Access rule excluded service accounts

---

## Risk Impact
Describe the risk if unaddressed.

Example:
"Attackers could authenticate without MFA, increasing credential-stuffing success."

---

## Remediation / Hardening Actions
Provide recommended changes:

| Action | Priority | Owner |
|--------|---------|-------|
| Block legacy authentication | High | Security Team |
| Enforce MFA for all users | High | Identity Team |
| Add geolocation conditions | Medium | IAM |

---

## Lessons Learned
- What went well
- What delayed investigation
- What tooling or logging needs improvement
- How future incidents will be faster to resolve

---

## MITRE ATT&CK Mapping
| Tactic | Technique |
|--------|-----------|
| Credential Access | Valid Accounts |
| Initial Access | Phishing |
| Defense Evasion | Disable Security Tools |

---

## Evidence
Screenshots, redacted logs, or charts go here.
(Do not upload sensitive data.)
