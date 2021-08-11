# Repository Summary
* Docker  
* Docker Compose
* Microservices-architecture (Spring Boot - Java Framework)
* H2 In-Memory Database
* System Monitoring (Prometheus)
* Platform-Provided Service Discovery (Deployment infrastructure take care of service discovery)
* Service-discovery (Docker-DNS)
* API-gateway (NGINX)
* Shell Scripting

To destroy infrastructure run the following command in **Git Bash**:
```shell
docker-compose down -v
```
# Prometheus Instructions (System Monitoring using Prometheus)
**Start Docker Daemon:** If you're using Docker for Windows, Then simply start the desktop app installed in:
```shell
C:\Program Files\Docker\Docker\Docker Desktop.exe
```
Position yourself using **Git Bash** in the folder where `docker-compose.yml` file is:
```
cd DOCKER-COMPOSE_FILE_PATH
```
Mapping environment variables from the environment file to the docker-compose.yml file (Check how your docker-compose.yml will finally look like, after environment variables substitution)
```shell
docker-compose --env-file .env config
```
To set up infrastructure run the following command in **Git Bash**:
```shell
docker-compose up --build
```
Docker-compose services/containers listing (one service one container)
```shell
docker-compose ps
```
```shell
docker ps
```
