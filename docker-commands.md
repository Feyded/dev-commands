# Developer Commands Cheat Sheet

A simple reference for commonly used Docker commands.

---

## Docker Commands

### 1. Build and start services

Build Docker images before starting the services and attach to the current workspace:

```bash

# Build the image if didnt specify tag default is latest
docker build -t {APP_NAME}-web-app:{TAG} .

# Tag the image first argument is the your local image second is the docker hub repository
docker tag {USERNAME}/{APP_NAME}-web-app:{TAG} {USERNAME}/{APP_NAME}-web-app:{TAG}

# Push the image to docker hub
docker push {USERNAME}/{APP_NAME}-web-app:{TAG}

# Pull the image
docker pull {USERNAME}/{APP_NAME}-web-app:{TAG}

# Build images before starting the services (corrected the typo: --build instead of -build)
docker compose up --build -w

# Start services defined in docker-compose.yml and attach to the current workspace
docker compose up -w

# List all running Docker containers
docker ps

# Start an interactive bash session inside a running container
docker exec -it container_name /bin/bash
```
