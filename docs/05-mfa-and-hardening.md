# MFA & Hardening

## Controls
- Enable MFA for vault accounts where supported
- Use a strong master password
- Protect administrative functionality
- Disable unnecessary registration after account provisioning if appropriate
- Keep the host/container images patched
- Limit inbound firewall rules
- Review logs
- Remove unused services
- Protect backup files

## Validation
Document each control, why it was selected, and the test proving normal access still works.

## Evidence
Capture sanitized security settings and firewall/service state. Never include MFA recovery codes.
