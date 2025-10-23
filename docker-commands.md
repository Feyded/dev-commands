# Developer Commands Cheat Sheet

A simple reference for commonly used Docker commands.

---

## Docker Commands

### 1. Build and start services

Build Docker images before starting the services and attach to the current workspace:

```bash
docker compose up --build -w

# Start services defined in docker-compose.yml and attach to the current workspace
docker compose up -w

# List all running Docker containers
docker ps

# Start an interactive bash session inside a running container
docker exec -it container_name /bin/bash
```
