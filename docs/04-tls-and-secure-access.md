# TLS & Secure Access

## Objective
Ensure credentials are not transmitted over unencrypted HTTP across untrusted networks.

## Design
Place an HTTPS-capable reverse proxy in front of Vaultwarden or use another documented secure-access design appropriate for the environment.

## Validate
- Browser reports HTTPS
- Certificate is valid for the chosen name
- Plain HTTP is redirected or unavailable as designed
- Vaultwarden is not unintentionally exposed on unnecessary interfaces/ports

## Remote Access
Prefer a deliberately secured remote-access method rather than casually forwarding the application port to the public Internet.

## Evidence
Capture the HTTPS connection details without exposing private keys, tokens, or sensitive public configuration.
