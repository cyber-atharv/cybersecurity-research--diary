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
