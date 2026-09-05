# Enterprise Security Lab Architecture

## Objective
Create a small enterprise-style environment for learning how endpoint and server telemetry flows into SIEM/EDR platforms and how a SOC analyst investigates alerts.

## Planned Components
| Layer | Component | Purpose |
|---|---|---|
| Endpoint | Windows + Sysmon | Process, authentication, network, and system telemetry |
| Server | Linux | Server/security log collection |
| SIEM | Wazuh | Centralized security monitoring and analysis |
| EDR | LimaCharlie | Endpoint visibility and response concepts |
| Analyst | Security workstation | Investigation, hunting, and documentation |

## Security Principles
- Use isolated lab systems.
- Generate test activity only on authorized assets.
- Never commit credentials or API keys.
- Sanitize hostnames, usernames, addresses, and screenshots before publishing.
- Keep detection documentation reproducible and evidence-based.

## Data Flow
1. Endpoint/server generates security telemetry.
2. Security agents collect relevant events.
3. SIEM/EDR platform processes telemetry.
4. Detection logic identifies suspicious patterns.
5. Analyst validates context and severity.
6. Findings are documented in an incident report.
