# Docker Joomla — Local Development

Lightweight, reproducible local Joomla development environment using Docker (docker-compose).

## Overview
This repository provides a ready-to-run local Joomla environment with:
- Joomla 
- MariaDB
- phpMyAdmin 
- Persistent volumes for code and database

## Requirements
- Docker (>= 20.x) and Docker Compose (v2 recommended)
- Git (optional)

## Quick start
1. Clone this repository.
2. Create a `.env` (see example below).
3. Start services:
    ```
    docker compose up -d
    ```
4. Visit:
    - Joomla: http://localhost:8080
    - phpMyAdmin: http://localhost:8081
    - mailhog: http://localhost:8025

To stop and remove containers (keep volumes):
```
docker compose down
```

To remove containers and volumes:
```
docker compose down -v
```

## Example .env
```
MYSQL_DATABASE=joomla_db
MYSQL_USER=joomla_user
MYSQL_PASSWORD=joomla_password
MYSQL_ROOT_PASSWORD=root_password
```

## License
GPL v2 or later

That's it — start coding.