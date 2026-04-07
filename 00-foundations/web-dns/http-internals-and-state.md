# Stage 04: DNS, HTTP and the Web Architecture

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
HTTP/1.1-2-3 protocols, header injection, state management, cookies, SOP and CORS boundaries.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 04: DNS, HTTP and the Web Architecture`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-04` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T11:29:51+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2025-12-10T10:45:34+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2025-12-10T20:01:39+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2025-12-15T10:00:00+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2025-12-15T21:21:05+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-20T12:15:42+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-20T21:31:47+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-23T19:38:08+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-26T15:25:50+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-28T18:40:41+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-30T16:01:34+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-01-02T18:31:31+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-01-07T10:34:17+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-01-09T10:00:00+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-09T19:16:05+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-01-11T16:11:33+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-15T14:49:34+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-18T13:26:08+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-20T20:01:15+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-01-24T11:21:34+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-01-28T17:39:25+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-01-31T11:44:51+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-02-01T12:45:42+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-02-03T15:34:25+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-02-07T11:29:51+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-02-08T13:25:34+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-02-09T20:50:40+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-02-11T17:39:25+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-02-12T18:15:14+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-02-16T16:52:16+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-02-18T15:51:41+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-02-19T18:06:24+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-02-24T19:08:51+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-02-25T21:00:48+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-03-02T14:59:33+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-03-03T20:18:24+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-03-05T20:26:31+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-03-13T14:01:34+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-03-15T14:30:24+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-03-16T14:24:25+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-03-18T16:00:32+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-03-21T13:07:17+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-03-23T16:04:16+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-03-24T19:06:49+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-03-29T17:39:25+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-04-02T11:12:17+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-04-06T14:38:51+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-04-07T20:50:40+05:30 | TCP State Machine & Half-Open SYN Probing -->
