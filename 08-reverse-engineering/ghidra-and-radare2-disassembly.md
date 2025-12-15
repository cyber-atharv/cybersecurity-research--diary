# Stage 19: Reverse Engineering & Disassembly

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
Ghidra decompilation, Radare2 visual mode, x86/x64 calling conventions, and stack frame analysis.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 19: Reverse Engineering & Disassembly`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-19` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T18:15:06+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2025-12-10T16:16:49+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2025-12-13T11:12:17+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->

<!-- Node: 2025-12-15T16:46:15+05:30 | Container Breakout: Mounted docker.sock & Privileged Escapes -->
