# Stage 08: Nmap & Network Enumeration

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
TCP SYN vs Connect scans, OS fingerprinting, version detection engines, and custom Lua NSE scripts.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 08: Nmap & Network Enumeration`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-08` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T13:19:59+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-10T12:15:42+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-10T21:31:47+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-15T11:50:08+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-19T12:08:51+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-20T13:45:50+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-21T14:08:51+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2025-12-24T12:41:51+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2025-12-26T17:35:58+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2025-12-28T21:22:49+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-02T10:45:34+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-01-02T20:01:39+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-07T12:24:25+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-09T11:30:08+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-09T20:46:13+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-01-11T18:40:41+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->
