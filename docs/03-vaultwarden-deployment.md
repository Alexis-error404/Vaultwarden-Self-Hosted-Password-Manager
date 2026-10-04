# Vaultwarden Deployment

## Objective
Run Vaultwarden as a persistent containerized service.

## Build
1. Create a dedicated project directory.
2. Define persistent storage.
3. Configure Vaultwarden using documented environment settings.
4. Keep secrets outside Git.
5. Start the service.
6. Review container logs for startup errors.
7. Create only test data until backup/recovery is validated.

## Validation
```bash
docker compose ps
docker compose logs --tail=100
```

Verify the web vault loads through the intended access path.

## Evidence
Capture the sanitized Compose/service state, container health, and web-vault login page. Never capture a real vault password or recovery material.
