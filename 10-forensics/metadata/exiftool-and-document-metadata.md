# Stage 17: Metadata, ExifTool & Artifact Forensics

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
ExifTool inspection, PDF stream analysis, embedded GPS/author data extraction, and file triage pipelines.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 17: Metadata, ExifTool & Artifact Forensics`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-17` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T17:20:32+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2025-12-10T15:31:15+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2025-12-11T20:44:16+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2025-12-15T15:51:41+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2025-12-19T18:06:24+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2025-12-20T17:01:23+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2025-12-22T13:23:51+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2025-12-24T20:18:24+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2025-12-28T10:47:17+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2025-12-29T15:24:16+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-01-02T14:14:07+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-01-03T15:22:08+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-01-07T16:25:58+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-01-09T14:46:41+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-01-10T18:03:42+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-01-12T13:26:08+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-01-17T16:45:50+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-01-20T12:08:51+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-01-21T17:35:50+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-01-24T20:01:15+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-01-30T13:08:51+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-01-31T18:40:32+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-02-01T18:36:23+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-02-05T15:25:59+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-02-07T17:20:32+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-02-09T14:20:16+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-02-10T17:32:07+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->
