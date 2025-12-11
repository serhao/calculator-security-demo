# Security Scanning

## Overview
This repository uses three types of security scanning:

### SAST (Static Analysis with CodeQL)
- Scans source code for vulnerabilities
- Runs on push to main branch
- Checks for: SQL injection, XSS, hardcoded secrets, data flow vulnerabilities
- Artifacts: See GitHub Security tab

### SCA (Dependency Check)
- Scans Python packages for known CVEs
- Runs on push to main branch
- Checks for: Outdated dependencies, known CVEs, vulnerable packages
- Artifacts: sca-reports

### DAST (Live Application with ZAP)
- Tests running application for vulnerabilities
- Runs on push to main branch
- Checks for: Missing security headers, injection flaws, configuration issues
- Artifacts: zap-baseline-reports, zap-fullscan-reports

## Understanding Results
See SCAN_ANALYSIS.md for detailed findings

## Reporting Vulnerabilities
Please email security@example.com
