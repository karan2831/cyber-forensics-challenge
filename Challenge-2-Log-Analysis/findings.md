# Challenge 2 — Log Analysis Findings

## 1. Investigation Overview

This investigation analyzed endpoint, execution, and Windows forensic
artifacts to ascertain which system showed evidence of compromise and
to reconstruct how suspicious activity occurred.

The investigation focused on endpoint identification, executable
execution, Windows Prefetch artifacts, and timeline reconstruction.

---

## 2. Affected Endpoint

The endpoint associated with the investigated activity was:

| Field | Value |
|---|---|
| Endpoint ID | EPOC6Y4R |
| Host | host-e783 |
| MAC Address | A2:DC:C5:9F:EC:E9 |
| Unit | unit-charlie |

The available evidence supports identifying `EPOC6Y4R` as the endpoint
requiring investigation.

---

## 3. Evidence Analyzed

The investigation used the following evidence sources:

- Endpoint security logs
- Web activity logs
- USB event logs
- Windows Prefetch artifacts
- PECmd output
- PECmd timeline
- Timeline Explorer
- Executable execution records

These artifacts were correlated rather than relying on a single log
source.

---

## 4. Windows Prefetch Analysis

Windows Prefetch artifacts were examined using PECmd.

Six Prefetch files were available for analysis, including:

- `AEXINSTALLPRECHECK.EXE`
- `CD DRIVE.EXE`
- `KFJUUWORMM.EXE`
- `MHYMHQ...EXE`
- `MQMJXFJVPE.EXE`
- `YVWPF...EXE`

The most significant artifact was:

`KFJUUWORMM.EXE-114B5780.pf`

The Prefetch record showed:

- Run Count: 1
- Last Run: `2026-07-08 07:05:02`
- Execution path:

```text
...\USERS\CLKSTG_3CDU\APPDATA\LOCAL\TEMP\_READY_TEMP_\KFJUUWORMM.EXE
