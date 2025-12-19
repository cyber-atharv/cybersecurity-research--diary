# Stage 17: Metadata, ExifTool & Artifact Forensics

> *"A comprehensive understanding of the underlying system eliminates the need to guess. When the architecture is mapped, the vulnerability reveals itself as a mathematical certainty."*

## 1. Tactical Overview
ExifTool inspection, PDF stream analysis, embedded GPS/author data extraction, and file triage pipelines.

## 2. Technical Invariants & Vulnerability Primitives
- **Core Subsystem**: `Stage 17: Metadata, ExifTool & Artifact Forensics`
- **Attack Surface**: Enumerate untrusted input boundaries, protocol parsers, and privilege transitions.
- **Telemetry Footprint**: Kernel audit logs, process creation events, network packet metadata.

## 3. Defensive Mirror
| Attack Primitive | Telemetry Generated | Log Source | Mitigation |
|---|---|---|---|
| `stage-17` | State violation / abnormal syscall | Auditd / Sysmon EID 1 | Parameterized APIs & capability boundaries |

<!-- Node: 2025-12-08T17:20:32+05:30 | ExifTool Deep Inspection: Forensic Provenance in Images -->

<!-- Node: 2025-12-10T15:31:15+05:30 | Volatility 3 Kernel Memory Dump & VAD Tree Inspection -->

<!-- Node: 2025-12-11T20:44:16+05:30 | Ghidra Decompilation & Control Flow Graph Reconstruction -->

<!-- Node: 2025-12-15T15:51:41+05:30 | ROP Chain Construction & Ret2libc Exploitation -->

<!-- Node: 2025-12-19T18:06:24+05:30 | Kerberoasting SPNs & Offline TGS Ticket Cracking -->
