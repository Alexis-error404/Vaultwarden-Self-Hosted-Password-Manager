# Self-Hosted Password Manager — Vaultwarden

**Security Engineering • Docker • Linux • Identity**

## Project Summary
Deploy a private password-management service while treating security, encrypted transport, access control, backup, recovery, and patching as first-class requirements.

This repository is structured as a portfolio project: architecture, implementation, validation, security considerations, troubleshooting, and screenshot evidence are documented so the work can be reproduced and discussed in a technical interview.

## Architecture
```text
User Devices
     |
 HTTPS / TLS
     |
Reverse Proxy
     |
Vaultwarden Container
     |
Encrypted Vault Data
     |
Backup + Recovery
```

## Core Skills
- Linux
- Docker
- Vaultwarden
- TLS
- Reverse Proxy
- MFA
- Backups
- Least Privilege
- Security Hardening

## Project Documentation
1. [Architecture And Threat Model](docs/01-architecture-and-threat-model.md)
2. [Linux And Docker](docs/02-linux-and-docker.md)
3. [Vaultwarden Deployment](docs/03-vaultwarden-deployment.md)
4. [Tls And Secure Access](docs/04-tls-and-secure-access.md)
5. [Mfa And Hardening](docs/05-mfa-and-hardening.md)
6. [Backup And Recovery](docs/06-backup-and-recovery.md)
7. [Maintenance And Troubleshooting](docs/07-maintenance-and-troubleshooting.md)
8. [Screenshot Evidence](images/README.md)

## Validation Standard
For every major component I document:
1. **Purpose** — why the component exists.
2. **Configuration** — how I deployed it.
3. **Validation** — commands/tests proving it works.
4. **Troubleshooting** — likely failure points and diagnostic steps.
5. **Security** — how access and exposure are reduced.
6. **Evidence** — sanitized screenshots of the completed work.

## Portfolio Safety
No real passwords, secrets, API tokens, private keys, product keys, recovery codes, personal data, or sensitive public-facing configuration should be committed.

## What This Project Demonstrates
Rather than only listing technologies on a résumé, this lab provides evidence of planning, implementation, administration, documentation, troubleshooting, and security-minded decision making.

## Author
**Alexis Wiscovitch** — [@Alexis-error404](https://github.com/Alexis-error404)
