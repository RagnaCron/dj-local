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
1. Clone or create project directory.
2. Create a `.env` (see example below).
3. Start services:
    ```
    docker compose up -d
    ```
4. Visit:
    - Joomla: http://localhost:8080
    - phpMyAdmin: http://localhost:8081

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
MYSQL_DATABASE=jo_database
MYSQL_USER=jouser
MYSQL_PASSWORD=jo_password
MYSQL_ROOT_PASSWORD=root_password
```

## License
GPL v2 or later

That's it — start coding.