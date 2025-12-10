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
