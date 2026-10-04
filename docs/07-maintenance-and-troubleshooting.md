# Maintenance & Troubleshooting

## Routine
- Review host updates
- Review container image updates
- Check service health/logs
- Verify storage capacity
- Confirm backups complete
- Periodically test recovery
- Review exposed ports and accounts

## Troubleshooting
```bash
docker compose ps
docker compose logs --tail=100
df -h
ss -tulpn
systemctl --failed
```

Troubleshoot in layers: host -> network -> container runtime -> container -> proxy/TLS -> client.

## Change Record
For meaningful changes, record date, reason, implementation, validation, and rollback approach.
