# Stage 02: Linux Command Line & Shell Thinking

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Grep regex optimization, stream processing with awk/sed, process signals, and shell reasoning.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 02: Linux Command Line & Shell Thinking`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-02` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T10:34:17+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2025-12-10T10:00:00+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2025-12-10T19:16:05+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2025-12-13T19:56:33+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2025-12-15T20:26:31+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2025-12-20T11:30:08+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2025-12-20T20:46:13+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2025-12-23T14:49:34+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2025-12-26T14:20:16+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2025-12-28T17:32:07+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-30T10:00:00+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-01-02T17:46:57+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-01-05T20:09:25+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-01-07T21:00:48+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-01-09T18:31:31+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-01-11T14:50:59+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-01-15T10:00:00+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-01-18T11:43:34+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-20T18:40:41+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-24T10:00:00+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-28T14:38:51+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-01-31T10:39:17+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-02-01T11:50:08+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-02-03T13:23:51+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-02-07T10:34:17+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-02-08T10:00:00+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-02-09T19:45:06+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-02-11T14:38:51+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-02-12T17:30:40+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-02-16T15:09:42+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-02-18T15:09:07+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-02-19T16:45:50+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-02-24T13:07:17+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-02-25T20:05:14+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-03-02T13:54:59+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-03-03T18:35:50+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-03-05T19:31:57+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-03-13T10:00:00+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-03-15T13:45:50+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-03-16T12:41:51+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-03-18T15:15:58+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-03-20T20:40:59+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-03-23T14:33:42+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-03-24T18:01:15+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-03-29T14:38:51+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-04-01T20:44:16+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-04-06T11:37:17+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-04-07T19:45:06+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-04-13T15:25:59+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-04-15T14:24:25+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-04-20T12:11:34+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-04-23T10:00:00+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-04-24T18:15:06+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-04-26T17:41:49+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-04-29T10:00:00+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-05-03T14:08:51+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-05-06T15:14:51+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-05-09T13:23:51+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-05-12T13:01:34+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-05-16T15:25:59+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-05-20T10:00:00+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-05-20T19:16:05+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-05-24T14:35:50+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-05-26T14:02:08+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-05-27T19:06:49+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-06-01T17:10:59+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-06-04T12:15:42+05:30 | ROP Chain Construction & Ret2libc Exploitation -->
