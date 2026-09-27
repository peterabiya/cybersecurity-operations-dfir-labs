# Network Traffic Analysis — Suspicious HTTP Login Activity

## Objective

Analyze the supplied PCAP in Wireshark to understand the captured traffic, identify suspicious activity, and explain the security implications.

## Investigation Approach

I reviewed the **Protocol Hierarchy, Endpoints, Conversations, TCP Streams, and HTTP Streams**. The capture contained TCP, HTTP and DNS activity between internal and external systems.

During stream analysis, the domain `gtbank-secure.net` stood out because it appeared to imitate a banking-related service. Following the TCP stream exposed a `GET /login.php` request and a page titled **GTBank Secure Login**. A subsequent `POST /login.php` contained submitted credentials in cleartext over HTTP.

## Findings

The activity was assessed as suspicious and consistent with a possible phishing or credential-harvesting page because:

- the domain imitated a banking-related name;
- the page requested a username and password;
- the credentials were transmitted in cleartext;
- the communication used HTTP rather than HTTPS; and
- the login page was unusually basic.

## Security Impact

In a real environment, this pattern could contribute to unauthorized account access, theft of sensitive information, financial fraud, and identity theft.

## Recommendations

- Verify URLs before submitting sensitive information.
- Use HTTPS for authentication and sensitive data transmission.
- Increase user awareness of fake login pages and phishing.
- Use stronger authentication controls where possible.

## What This Lab Demonstrates

This exercise demonstrates PCAP triage, HTTP/TCP stream inspection, suspicious-domain analysis, cleartext credential identification, and evidence-based reporting with Wireshark.
