# Stage 12: XSS & Client-Side Security

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Reflected/Stored/DOM XSS, context sinks, CSP bypasses, DOMPurify, and trusted types.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 12: XSS & Client-Side Security`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-12` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T15:09:07+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-10T13:45:50+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-11T14:08:51+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->

<!-- Node: 2025-12-15T13:40:16+05:30 | SPF, DKIM, and DMARC Header Authentication Analysis -->

<!-- Node: 2025-12-19T14:50:59+05:30 | PE File Header Forensics: Import Tables & Entropy Analysis -->
