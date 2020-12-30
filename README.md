## Docker with Laravel 8  

Docker clean Laravel 8 installation with PostgreSQL, Redis and nginx

## Installation

1. Setup .env  
2. `docker-compose up -d --build`
2. `docker-compose run --rm composer install`        
3. `docker-compose run --rm key:generate`  
3. `docker-compose run --rm artisan migrate`  


-----

- [Docker guide](./guide/docker.md)

-----