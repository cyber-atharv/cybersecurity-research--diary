# Stage 05: Windows & Linux Security Internals

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Linux POSIX capabilities, SUID, Windows access tokens, Registry run keys, and audit logging.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 05: Windows & Linux Security Internals`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-05` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T11:50:08+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2025-12-10T11:14:51+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2025-12-10T20:17:56+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2025-12-15T10:34:17+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-19T10:00:00+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-20T12:44:59+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-21T10:00:00+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-24T10:00:00+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-26T16:04:07+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-28T19:27:58+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2025-12-30T19:08:51+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-01-02T19:00:48+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-01-07T10:55:34+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-09T10:29:17+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->
