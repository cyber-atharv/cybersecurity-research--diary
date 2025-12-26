# Stage 06: Cryptography & Encoding

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Encoding vs Hashing vs Encryption, AES padding oracles, RSA low-exponent attacks, and PKI.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 06: Cryptography & Encoding`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-06` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T12:24:25+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2025-12-10T11:30:08+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2025-12-10T20:46:13+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-15T10:55:34+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-19T10:47:17+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-20T13:00:16+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-21T11:27:17+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-24T10:58:17+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-26T16:30:24+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->
