## Base Image Selection
- Backend: `node:14` for compatibility with the application's dependencies.
- Frontend: `nginx:alpine` for a lightweight and efficient web server.
- Database: `mongo:4.4` for reliable MongoDB service.

## Dockerfile Directives
- Used `COPY` to add source code and dependencies.
- Used `RUN` to install necessary packages.
- Used `EXPOSE` to open required ports.
- Used `CMD` to start the application.

## Docker-compose Networking
- Defined services and set up a bridge network for inter-service communication.
- Allocated ports for frontend and backend services.

## Docker-compose Volume Definition
- Used a named volume `mongo-data` to persist MongoDB data across container restarts.

## Git Workflow
- Followed a systematic approach with descriptive commits.
- Structured the repository for clarity and ease of navigation.

## Debugging Measures
- Checked logs using `docker logs container_id to troubleshoot issues.
- Ensured network settings allowed proper communication between containers.

