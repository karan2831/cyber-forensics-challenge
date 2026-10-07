# Cyber Forensics & Incident Analysis Challenges

A hands-on cybersecurity investigation covering malware analysis,
digital forensics, endpoint investigation, log correlation, and
audio forensics.

## Challenges

### 01 — Malware Analysis

Analysis of a suspicious Windows executable using static and dynamic
malware-analysis techniques.

**Tools:**
- Detect It Easy
- PEStudio
- Ghidra
- CAPA
- Procmon

**Key Areas:**
- PE-file analysis
- Static malware analysis
- Capability identification
- Reverse engineering
- Runtime behavior
- Process and file activity
- Indicators of compromise

---

### 02 — Log Analysis: Ascertain Who Is Compromised and How

Investigation of endpoint and activity logs to identify the affected
system and reconstruct suspicious activity.

**Evidence Analyzed:**
- Endpoint security logs
- Web activity logs
- USB events
- Windows Prefetch artifacts
- PECmd output
- Timeline Explorer
- Executable execution records

**Key Areas:**
- Endpoint identification
- Timeline reconstruction
- Cross-artifact correlation
- Suspicious execution analysis
- IOC correlation
- Compromise assessment
- Evidence validation

**Primary Endpoint Investigated:**

`EPOC6Y4R` / `host-e783`

---


---

## Investigation Workflow

```text
Evidence Collection
        ↓
Initial Triage
        ↓
Malware Analysis
        ↓
Log & Artifact Analysis
        ↓
Timeline Reconstruction
        ↓
Audio Forensics
        ↓
Cross-Evidence Correlation
        ↓
Findings
        ↓
Forensic Documentation
