 Network Security

Projects and notes related to network defence, packet analysis, firewalls, protocols, and traffic flow. Focus areas include Wireshark investigations, port/protocol behaviour, and network-based detection logic.
# Network Security Analysis – [Title of Investigation]

## Summary
Brief explanation of the network-related issue, detection, or behaviour being investigated.

Example:
"Outbound traffic spike to unfamiliar IP range flagged by firewall logs."

---

## Objective
- Identify whether the traffic is expected or suspicious
- Determine associated services, ports, and protocols
- Analyse packet contents or metadata for malicious indicators
- Document findings for SOC escalation or closure

---

## Tools and Data Sources
- Wireshark (packet capture)
- Firewall logs (Fortinet, Cisco, Azure, etc.)
- Netstat / ss / lsof outputs
- OSINT (IP lookups, domain reputation)
- DNS logs

---

## Technical Context

| Protocol | Port | Expected Use | Notes |
|----------|------|--------------|------|
| HTTP | 80 | Web browsing | Unencrypted |
| HTTPS | 443 | Web browsing | Encrypted |
| DNS | 53 | Name resolution | Could be exfiltration |
| SSH | 22 | Remote admin | Check source |

(Add or modify based on case)

---

## Investigation Steps

1. Captured traffic using Wireshark / PCAP
2. Filtered using:
   - `tcp.port == 443`
   - `ip.addr == [suspicious IP]`
   - `http.request.method == "POST"`
3. Correlated with firewall logs
4. Performed WHOIS/IP OSINT checks
5. Verified process associated with traffic (if endpoint access available)

---

## Findings

Example:
- 54 connections in 2 minutes to IP 104.78.X.X
- Traffic originated from PowerShell process
- Domain reputation shown as "Malicious" on VirusTotal
- No business case for asset communicating externally

---

## Risk Impact
- Data exfiltration
- Command-and-control communication
- Credential theft
- Shadow IT remote control tools

---

## Recommended Actions
| Action | Priority | Owner | Status |
|--------|---------|------|-------|
| Block outbound to IP | High | Network | Done |
| Isolate endpoint | High | SOC | Done |
| Reset credentials | Medium | IAM | Pending |
| Add alert for port behaviour | Medium | SIEM | Open |

---

## MITRE ATT&CK Mapping
| Tactic | Technique |
|--------|----------|
| Command and Control | Web Protocols |
| Exfiltration | Exfiltration Over Alternative Protocol |

---

## Lessons Learned
- Was logging sufficient?
- Could detection be faster?
- Was firewall rule appropriate?
- Did user awareness fail or succeed?

---

## Evidence
Attach redacted PCAP screenshots, OSINT reports, firewall logs.
Do not upload sensitive data.
