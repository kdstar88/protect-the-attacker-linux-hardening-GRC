# Protect the Attacker – Linux System Hardening & GRC Audit

## Cybersecurity Project

A practical GRC-focused Linux security assessment and hardening project performed on a Kali Linux virtual machine.

The project followed a structured security-hardening lifecycle:

**Audit → Analyze → Remediate → Verify → Re-audit**

## Objectives

- Assess the security posture of a Kali Linux system
- Identify and prioritize security findings
- Map selected findings to CIS Benchmarks and NIST 800-171
- Implement appropriate security hardening measures
- Verify implemented controls
- Document the results and perform a final re-audit

## Tools & Frameworks

- Kali Linux
- Lynis 3.1.6
- CIS Benchmarks
- NIST 800-171
- Fail2Ban
- debsums
- systemd

## Key Results

| Metric | Result |
|---|---:|
| Initial Lynis Hardening Index | 65 |
| Lowest observed index | 62 |
| Intermediate verified index | 63 |
| Final Hardening Index | 68 |
| Improvement vs. baseline | +3 |
| Final Lynis tests | 271 |

## Security Controls Implemented

- UMASK hardened to 027
- Fail2Ban enabled and verified with SSH jail
- Unnecessary ATFTP server component removed
- File integrity verification with debsums
- Security and maintenance utilities installed
- Login warning banners strengthened

## GRC Approach

The project focused not only on increasing the Lynis score, but on evaluating whether individual security controls were appropriate for the intended system.

Findings were analyzed, prioritized, remediated where appropriate, verified, and documented.

## Project Report

The complete project report documents the audit methodology, findings, remediation activities, verification steps and final results.

The report is available in the `report` directory.

## Risk Register

The project includes a risk register documenting selected security findings, framework mappings and mitigation considerations.

The risk register is available in the `risk-register` directory.

## Project Outcome

The final documented Lynis Hardening Index reached **68**, compared with an initial baseline of **65**, representing a **+3 point improvement**.

The project demonstrated a complete security hardening workflow from assessment and risk analysis through remediation, verification and final re-audit.
