Here’s an improved and well-structured guide for Docker commands:

# Docker Command Reference Guide

A concise guide to commonly used Docker commands for building, managing, and deploying containerized applications.

---

## Docker Basics
1. **`docker --version`**: Verifies the Docker installation and shows the installed version.
2. **`docker info`**: Provides detailed information about the Docker installation, including system and resource usage.
3. **`docker images`**: Lists all locally available Docker images.
4. **`docker ps`**: Displays currently running containers.
5. **`docker ps -a`**: Shows all containers, including those that are stopped.

---

## Working with Images
6. **`docker pull <image_name>`**: Downloads a Docker image from Docker Hub or another registry.
7. **`docker build -t <image_name> .`**: Builds a Docker image from a `Dockerfile` in the current directory and tags it with a name.
8. **`docker rmi <image_name>`**: Removes a Docker image from the local system.

---

## Managing Containers
9. **`docker run <image_name>`**: Creates and starts a container from a specified image.
10. **`docker run -d <image_name>`**: Runs a container in detached mode (in the background).
11. **`docker run -p <host_port>:<container_port> <image_name>`**: Runs a container and maps its internal port to a host machine port.
12. **`docker exec -it <container_id> <command>`**: Executes a command inside a running container (e.g., starting a bash shell).
13. **`docker stop <container_id>`**: Stops a running container gracefully.
14. **`docker kill <container_id>`**: Forces a running container to stop immediately.
15. **`docker rm <container_id>`**: Deletes a stopped container.

---

## Inspecting Containers
16. **`docker logs <container_id>`**: Displays the logs from a container.
17. **`docker inspect <container_id>`**: Shows detailed information about a specific container or image.
18. **`docker stats`**: Monitors live resource usage statistics of running containers.

---

## Volume and Network Management
19. **`docker volume ls`**: Lists all Docker volumes.
20. **`docker volume create <volume_name>`**: Creates a new volume.
21. **`docker volume rm <volume_name>`**: Removes a specific volume.
22. **`docker network ls`**: Lists all Docker networks.
23. **`docker network create <network_name>`**: Creates a custom network.
24. **`docker network rm <network_name>`**: Deletes a specified network.

---

## Advanced Commands
25. **`docker commit <container_id> <new_image_name>`**: Saves the changes in a container as a new image.
26. **`docker save -o <file_name> <image_name>`**: Exports a Docker image to a file.
27. **`docker load -i <file_name>`**: Loads a Docker image from a saved file.
28. **`docker system prune`**: Cleans up unused Docker objects, including stopped containers, dangling images, and unused networks.
29. **`docker-compose up`**: Builds and starts services defined in a `docker-compose.yml` file.
30. **`docker-compose down`**: Stops and removes services defined in a `docker-compose.yml` file.

---

## Debugging and Troubleshooting
31. **`docker top <container_id>`**: Displays the running processes inside a container.
32. **`docker diff <container_id>`**: Shows changes made to a container's filesystem.
33. **`docker restart <container_id>`**: Restarts a container.
34. **`docker events`**: Streams real-time events from the Docker daemon.

---

This guide is designed to help you quickly understand and use Docker commands for your containerized workflows. Bookmark it for easy reference!
