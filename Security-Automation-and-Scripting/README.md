Security Automation and Scripting

This section contains Python and PowerShell scripts created to automate security tasks, support SOC workflows, and improve investigation efficiency.

Example automation areas may include:

- Log parsing and filtering
- IOC extraction using regex
- VirusTotal, Shodan, or API lookups
- Automated case evidence export
- Bulk file or log manipulation
- Enrichment of alerts with contextual data

The focus is on building small, practical tools that support Blue Team operations rather than large engineering projects.


# Security Automation Case – [Script/Tool Name]

## Summary
Short explanation of the security problem the script solves.

Example:
"A PowerShell script created to automatically extract failed authentication attempts and export them for further triage."

---

## Objective
- Reduce manual workload for SOC analysts
- Automate repetitive investigation tasks
- Standardise data format for easier analysis

---

## Script Language
- [ ] Python
- [ ] PowerShell
- [ ] Other: ___________

---

## Problem Being Solved
Describe the manual task and why automating matters.

Example:
"Manually searching Event Viewer for login failures takes time and results may be inconsistent across analysts."

---

## Inputs & Outputs

| Input Source | Format | Description |
|--------------|---------|-------------|
| Log file | .evtx | Windows log export |
| API request | JSON | VirusTotal lookup |
| PCAP file | Packet Data | For parsing |

| Output | Format | Purpose |
|--------|--------|--------|
| CSV | Structured export |
| JSON | Application use |
| Console output | Analyst triage |

---

## Code Snippet (Key Section Only)

```python
# Python Code Example
# (Paste only key logic, not entire file)
