# Enterprise SIEM + EDR Security Lab

## Overview
A defensive cybersecurity portfolio lab designed to demonstrate SOC analyst workflows across centralized logging, endpoint telemetry, alert triage, investigation, detection engineering, and incident documentation.

This repository is structured around tools and skills I am developing, including **Wazuh, LimaCharlie, Windows, Linux, Sysmon, SIEM, EDR, log analysis, and incident response**.

> All attack simulation and testing should be performed only against systems I own or am explicitly authorized to test.

## Career Skills Demonstrated
- Security Operations Center (SOC) monitoring
- SIEM and EDR telemetry
- Windows and Linux security logging
- Sysmon event analysis
- Alert triage and investigation
- Detection engineering
- Incident response documentation
- MITRE ATT&CK mapping
- Threat hunting and log correlation

## Target Architecture
```text
                 +-------------------+
                 | Analyst Workstation|
                 +---------+---------+
                           |
                    SIEM / EDR Console
                           |
             +-------------+-------------+
             |                           |
      Windows Endpoint              Linux Server
      + Sysmon / Agent              + Security Agent
             |                           |
             +--------- Telemetry -------+
                           |
                 Centralized Detection
```

## Investigation Workflow
**Generate authorized test activity → Collect telemetry → Detect → Triage → Investigate → Contain/Recommend → Document**

## Planned Scenarios
1. Repeated failed authentication / brute-force-style lab activity
2. Suspicious PowerShell behavior in a controlled endpoint
3. New process / persistence-related telemetry
4. Unusual outbound network connection
5. Suspicious file or hash investigation

## Repository Structure
- `docs/architecture.md` — lab design and components
- `detections/` — detection-rule documentation
- `incidents/` — SOC incident-report templates
- `queries/` — reusable hunting/query notes
- `screenshots/` — sanitized evidence to add later

## Evidence Policy
Real screenshots, alert IDs, event counts, and findings will be added later. This repository does not fabricate lab results.

## Resume-Ready Summary
**Enterprise SIEM + EDR Lab** — Built a security operations lab to centralize Windows/Linux telemetry, investigate security alerts, correlate logs, develop detections, and document incidents using SOC-style workflows with SIEM/EDR technologies.

## Status
**In development — portfolio documentation and evidence collection ongoing.**
