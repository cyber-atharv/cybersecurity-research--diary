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

<!-- Node: 2026-01-09T19:32:22+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-01-11T16:45:50+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-01-15T17:20:51+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-01-18T14:24:25+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-01-20T20:48:32+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-01-24T12:08:51+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-01-28T19:03:42+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-01-31T12:10:08+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-02-01T13:19:59+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-02-03T16:33:42+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-02-07T11:50:08+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-02-08T15:14:51+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-02-09T21:16:57+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-02-11T19:03:42+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-02-12T18:31:31+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-02-16T17:50:33+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-02-18T16:25:58+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-02-19T18:40:41+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-02-25T10:00:00+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-02-25T21:21:05+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-03-02T15:25:50+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-03-03T21:03:41+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-03-05T21:00:48+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-03-13T16:08:51+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-03-15T14:46:41+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-03-16T15:09:42+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-03-18T16:16:49+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-03-21T16:01:34+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-03-23T16:56:33+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-03-24T19:45:06+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-03-29T19:03:42+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-04-02T12:11:34+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-04-06T16:02:08+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-04-07T21:16:57+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-04-13T17:35:50+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-04-15T16:52:16+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-04-20T15:34:25+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-04-23T15:14:51+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-04-24T19:31:57+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-04-26T19:10:40+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-04-29T11:44:51+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-05-03T18:03:42+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-05-06T20:15:42+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-05-09T16:33:42+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-05-12T17:39:25+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-05-16T17:35:50+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-05-20T11:14:51+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-05-20T20:17:56+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-05-24T15:51:41+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-05-26T17:10:59+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-05-27T20:50:40+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-06-01T20:05:50+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->

<!-- Node: 2026-06-04T13:29:33+05:30 | Detection Engineering: Crafting Sigma Rules for EDR Telemetry -->

<!-- Node: 2026-06-05T11:31:34+05:30 | Independent Threat Assessment & Zero-Knowledge Architecture Triage -->

<!-- Node: 2026-06-09T10:00:00+05:30 | Memory Paging & Page Table Walk analysis under Ring 0 -->

<!-- Node: 2026-06-10T19:56:33+05:30 | Stream Filtering & PCRE Flag Optimization -->

<!-- Node: 2026-06-13T20:48:32+05:30 | TCP State Machine & Half-Open SYN Probing -->

<!-- Node: 2026-06-17T19:08:51+05:30 | HTTP Header Injection & CRLF Smuggling Dynamics -->

<!-- Node: 2026-06-19T15:30:24+05:30 | POSIX Capabilities vs SUID Binary Exploitation -->

<!-- Node: 2026-06-21T16:04:07+05:30 | RSA Low Public Exponent & Coppersmith Attack Vectors -->

<!-- Node: 2026-06-23T17:39:25+05:30 | Certificate Transparency Logs for Subdomain Enumeration -->

<!-- Node: 2026-06-28T10:47:17+05:30 | Nmap Scripting Engine (NSE) Lua Engine Deconstruction -->

<!-- Node: 2026-06-29T15:24:16+05:30 | JavaScript Sourcemap Unpacking & Endpoint Extraction -->

<!-- Node: 2026-06-30T20:01:15+05:30 | UNION-based SQLi Column Alignment & Schema Dumping -->

<!-- Node: 2026-07-04T10:00:00+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2026-07-10T15:09:25+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2026-07-12T14:46:41+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2026-07-15T10:00:00+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2026-07-15T21:21:05+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2026-07-20T17:32:07+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->

<!-- Node: 2026-07-23T17:35:58+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2026-07-24T21:22:49+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2026-07-25T21:00:48+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2026-07-28T17:39:25+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2026-07-29T20:05:14+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2026-08-04T11:29:51+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->
