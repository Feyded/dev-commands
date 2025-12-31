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

# Start or update containers
docker compose up -d

# View logs
docker compose logs -f

# Shows only running containers
docker ps -a

# Shows all containers, including stopped ones
docker ps

# List all images
docker images ls

# Stop the specific container
docker stop container_name

# Removing the container (info) Only works if the container is stopped.
docker rm washmate-api

# Remove a specific image (info) remove first the container
docker rmi docker_image

# Remove all unused images
docker image prune

# Start an interactive bash session inside a running container
docker exec -it container_name /bin/bash
```
