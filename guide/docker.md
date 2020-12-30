## Prerequisites
- [Docker MacOS](https://docs.docker.com/docker-for-mac/install/)
- [Docker Windows](https://docs.docker.com/docker-for-windows/install/)

## Installation
1. Run `docker-compose up -d --build`
2. Run `docker-compose run --rm composer install`
3. Run `docker-compose run --rm npm install`
4. Done, your Docker instance should be now running.

Link to laravel instance [http://localhost:8080](http://localhost:8080)


> **Starting Docker**
>
> Command: `docker-compose up -d --build` is used only during initial run. The following spin-ups should be done using: `docker-compose up -d`

## Commands
- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 

## Containers
- **nginx**:stable-alpine - `:8080`
- **postgres**:9.5-alpine - `:5432`
- **php**:7.4-fpm-alpine - `:9000`
- **npm**:lts
- **composer**:latest
- **artisan**

> **Notes**:
>
> The docker volume `postgres` persists any updates made by laravel
to the database. [Learn more about docker volumes](https://github.com/docker/docker.github.io/blob/master/storage/volumes.md)
