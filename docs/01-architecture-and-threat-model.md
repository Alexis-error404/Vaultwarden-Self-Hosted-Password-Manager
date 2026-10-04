# Architecture & Threat Model

## Objective
Design the password-manager deployment before installation.

## Components
- Linux host
- Docker/Compose
- Vaultwarden container
- persistent application data
- HTTPS/reverse-proxy layer
- backup destination
- authorized client devices

## Assets to Protect
Vault data, administrative access, configuration secrets, backup data, TLS/private-key material, and host access.

## Primary Risks
| Risk | Control |
|---|---|
| Credential compromise | Strong unique credentials + MFA |
| Exposed admin interface | Restrict/disable unnecessary administrative exposure |
| Unencrypted transport | HTTPS/TLS |
| Host compromise | Patching, firewall, least privilege |
| Data loss | Tested backups |
| Secret leakage in Git | Never commit secrets; use environment/config separation |

## Trust Boundaries
Document which traffic remains inside the trusted LAN, which components can reach the Internet, and how remote access is handled. Avoid direct Internet exposure unless it is intentionally designed and hardened.

## Evidence
Capture a sanitized architecture diagram and host/network overview.
