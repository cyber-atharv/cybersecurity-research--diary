# Stage 11: Authentication & Authorization

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Session fixation, MFA logic flaws, IDOR matrix testing, and horizontal/vertical privilege escalation.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 11: Authentication & Authorization`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-11` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T14:35:50+05:30 | Horizontal vs Vertical IDOR Access Control Matrix -->

<!-- Node: 2025-12-10T13:29:33+05:30 | DOM-based XSS: Analysis of Dangerous JavaScript Sinks -->

<!-- Node: 2025-12-11T12:41:34+05:30 | SSRF to AWS IMDSv2 vs GCP Metadata Token Exfiltration -->

<!-- Node: 2025-12-15T13:19:59+05:30 | GraphQL Query Batching & Introspection Schema Extraction -->
