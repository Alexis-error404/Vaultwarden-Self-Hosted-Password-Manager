# Linux & Docker Foundation

## Objective
Prepare a patched Linux host and container runtime.

## Build
1. Install a supported Linux server distribution.
2. Apply system updates.
3. Configure a descriptive hostname.
4. Review network addressing.
5. Install Docker Engine and Compose using the vendor-supported method for the selected distribution.
6. Configure only required administrative users.
7. Verify Docker.

## Validation
```bash
hostname
ip addr
docker --version
docker compose version
docker ps
```

## Security
Do not expose the Docker socket remotely. Treat membership in privileged container-management groups as administrative access.

## Evidence
Capture OS information, Docker version, running service status, and sanitized network configuration.
