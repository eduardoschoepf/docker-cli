# Docker CLI Guide
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository provides a comprehensive guide to using Docker Command-Line Interface (CLI) commands.

## Table of Contents

- [Installation](#installation)
- [Basic Docker Commands](#basic-docker-commands)
- [Working with Containers](#working-with-containers)
- [Working with Images](#working-with-images)
- [Building Images](#building-images)
- [Managing Volumes](#managing-volumes)
- [Docker Compose](#docker-compose)
- [Contributing](#contributing)

## Installation

To install Docker, follow the [official installation guide](https://docs.docker.com/get-docker/).

Verify your installation with:
```
docker --version
````

## Basic Docker Commands

Check Docker Version
```
docker --version
```

Display System-wide Information
```
docker info
```

## Working with Containers

Run a New Container
```s
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
````

Example:  
```
docker run -d -p 80:80 nginx
```

List Running Containers
```
docker ps
```

List All Containers
```
docker ps -a
```

Stop a Running Container
```
docker stop CONTAINER_ID
```

Start a Stopped Container
```
docker start CONTAINER_ID
```

Remove a Stopped Container
```
docker rm CONTAINER_ID
```

## Working with Images

List Docker Images
```
docker images
```

Pull an Image from Docker Registry
```
docker pull IMAGE_NAME
```

Remove a Docker Image
```
docker rmi IMAGE_NAME
```

## Building Images

Build an Image from a Dockerfile
```
docker build [OPTIONS] PATH | URL | -
```

Example:
```
docker build -t my-image:latest .
```

## Managing Volumes

Create a New Volume
```
docker volume create VOLUME_NAME
```

List All Volumes
```
docker volume ls
```

Remove a Volume
```
docker volume rm VOLUME_NAME
```

## Docker Compose

Start Services Defined in docker-compose.yml
```
docker-compose up
```

Stop and Remove Services
```
docker-compose down
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.
