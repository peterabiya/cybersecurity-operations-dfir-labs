# Cybersecurity Operations & DFIR Labs

A portfolio of hands-on investigations completed during the **VA Cybersecurity Mentorship Programme**. The repository documents practical work across network traffic analysis, SIEM investigation, SOC triage, digital forensics, incident response, and governance, risk and compliance (GRC).

The emphasis is not only on the final finding, but on the investigation process: reviewing evidence, forming and testing hypotheses, correlating activity across data sources, documenting conclusions, and recommending defensive actions.

## Lab Index

| # | Investigation | Focus | Tools / Evidence |
|---|---|---|---|
| 01 | [Network Traffic Analysis](01-network-traffic-analysis/) | Suspicious HTTP login traffic and credential exposure | Wireshark, PCAP, TCP/HTTP streams |
| 02 | [Splunk Brute-Force Investigation](02-splunk-brute-force-investigation/) | Windows authentication analysis and incident response | Splunk, Windows Event IDs, MITRE ATT&CK |
| 03 | [KudiPay Network Investigation](03-kudipay-network-investigation/) | Suspicious outbound HTTPS traffic and possible exfiltration | Wireshark, TCP streams, Conversations |
| 04 | [SOC Incident Triage](04-soc-incident-triage/) | Alert validation, attack-chain analysis, escalation | Windows Security Events, firewall/network evidence |
| 05 | [Digital Forensics](05-digital-forensics/) | Disk and memory artefact analysis | Autopsy, memory-analysis output |
| 06 | [Incident Response Capstone](06-incident-response-capstone/) | Cross-source breach reconstruction | Network, host logs, disk and memory evidence |
| 07 | [GRC Risk Assessment](07-grc-risk-assessment/) | Risk identification, scoring and treatment | Risk register, 5×5 risk matrix |

## Investigation Progression

```text
Network Traffic Analysis
        ↓
SIEM / Windows Log Investigation
        ↓
SOC Triage & Escalation
        ↓
Digital Forensics
        ↓
Incident Reconstruction & Response
        ↓
Risk Assessment & Control Improvement
```

## Skills Demonstrated

- SIEM investigation and log analysis with Splunk
- Windows Security Event analysis
- Network traffic and TCP-stream analysis with Wireshark
- SOC alert triage, disposition and escalation
- MITRE ATT&CK mapping
- Disk and memory forensic analysis
- Evidence correlation and attack-chain reconstruction
- Incident reporting and remediation planning
- Risk assessment, scoring and treatment decisions

## Evidence Approach

Screenshots are retained alongside the relevant investigation and placed within each README where they support the analysis. The scenarios and infrastructure shown are fictional or controlled mentorship/lab environments and are presented for portfolio and learning purposes.

## Programme

**VA Cybersecurity Mentorship Programme — Victor Akinode Initiatives**  
**Analyst:** Peter Abiya  
**Year:** 2026
