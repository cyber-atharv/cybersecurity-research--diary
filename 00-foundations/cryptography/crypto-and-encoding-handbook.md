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

<!-- Node: 2025-12-28T20:01:15+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-01-02T10:00:00+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-01-02T19:16:05+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-07T11:29:51+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-01-09T10:45:34+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-09T20:01:39+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-11T17:32:07+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-15T19:38:08+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-01-18T15:09:42+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-01-20T21:22:49+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-01-24T12:42:08+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-01-28T20:40:59+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-01-31T12:49:25+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-02-01T13:40:16+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-02-03T17:45:59+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-02-07T12:24:25+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-02-08T16:50:08+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-02-10T10:00:00+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-02-11T20:40:59+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-02-12T19:00:48+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-02-16T18:35:50+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-02-18T16:46:15+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->
