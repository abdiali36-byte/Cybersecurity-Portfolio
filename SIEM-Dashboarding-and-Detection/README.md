SIEM Dashboarding and Detection Engineering

Examples of log analysis, alert creation, KQL or SPL queries, dashboard designs, and detection engineering aligned with MITRE ATT&CK frameworks.

# SIEM Detection Case Study – [Detection Name / Alert Title]

## Summary
Short explanation of what the detection or alert is intended to identify.

Example:
"Detection created to identify multiple failed login attempts followed by a successful login."

---

## Objective
- Understand behaviour that triggers this detection
- Determine whether the logic reduces false positives
- Evaluate visibility and data sources required

---

## Data Sources Used
(Select or delete as relevant)

- Authentication logs
- Firewall logs
- DNS logs
- Endpoint security platform alerts
- Cloud identity logs
- Email security logs

---

## Query or Logic (If applicable)
Paste the query or describe the logical conditions the detection checks.

Example:


If you don’t have a query yet, write:
*Query to be added when SIEM platform is chosen.*

---

## Investigation Workflow
1. Alert received  
2. Correlated with user behaviour  
3. Checked device identity  
4. Validated source IP reputation  
5. Determined business context  

---

## Tuning & False Positive Considerations
- Which benign behaviours could trigger false alerts?
- Which sources of noise were identified?
- Who needs to be excluded (e.g., IT automation accounts)?

---

## Risk or Threat Addressed
Examples:
- Brute force attacks  
- Credential stuffing  
- Insider threat  
- Lateral movement  

---

## MITRE ATT&CK Mapping
| Tactic | Technique |
|--------|----------|
| [Add relevant mapping] | [Add technique] |

---

## Improvements / Next Iteration
- Add additional log correlation
- Visualize login patterns
- Create severity levels
- Add threshold logic

---

## Evidence (Optional)
- Dashboard UI screenshot
- Log snippet
- Timestamp examples
