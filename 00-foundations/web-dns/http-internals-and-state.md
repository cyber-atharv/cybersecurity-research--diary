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
