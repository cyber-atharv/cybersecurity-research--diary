# Stage 01: Computer & Security Foundations

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
CPU architecture, memory paging, user vs kernel ring transitions, and fault injection.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 01: Computer & Security Foundations`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-01` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T10:00:00+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2025-12-08T21:21:05+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2025-12-10T19:00:48+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2025-12-13T18:44:16+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2025-12-15T20:05:14+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2025-12-20T11:14:51+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2025-12-20T20:17:56+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2025-12-23T12:31:17+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-26T13:54:59+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-28T16:45:50+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-29T21:22:49+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-01-02T17:30:40+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-01-05T18:02:08+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-01-07T20:26:31+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-01-09T18:15:14+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-01-11T14:03:42+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-01-12T21:03:41+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-18T10:58:17+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-01-20T18:06:24+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-23T19:08:51+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-28T13:01:34+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-31T10:00:00+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-02-01T11:29:51+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-02-03T12:11:34+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-02-07T10:00:00+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-02-07T21:21:05+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-02-09T19:06:49+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-02-11T13:01:34+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->
