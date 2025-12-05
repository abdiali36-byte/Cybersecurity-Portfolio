 Identity and Access Security

Documentation and cases focused on identity protection, MFA enforcement, Conditional Access, account lockouts, and identity-based attack paths in modern cloud and hybrid environments.
# Identity & Access Investigation – [Title of Case]

## Summary
Brief overview of the identity-related issue, authentication error, or access misconfiguration identified.

Example:
"Multiple failed MFA prompts reported by user, suspected MFA fatigue attack."

---

## Objective
- Identify root cause of authentication failure
- Determine if access was legitimate or malicious
- Evaluate whether policies operated as intended

---

## Relevant Policies and Controls
Document the relevant IAM settings:

- Conditional Access rules (summary)
- MFA enforcement level (Per-user / Security defaults / Conditional)
- Role assignments
- Self-service password reset
- Legacy authentication blocked? (Yes/No)

---

## Investigation Steps
List your steps clearly:

1. Reviewed sign-in logs for geographic anomalies  
2. Checked device compliance  
3. Validated user agent strings  
4. Examined Conditional Access policy outcomes  
5. Compared access attempts against user behaviour  

---

## Findings
Summarise key outcomes.

Example:
- User received 14 MFA prompts in 4 minutes
- Device and IP unknown to tenant
- Policy did not challenge non-compliant device

---

## Ri
