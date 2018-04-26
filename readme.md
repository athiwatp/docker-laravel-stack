## Dev : docker + laravel

- [x] [Part 1 - development](https://medium.com/@acceth/laravel-docker-laradock-753382ee2292)
- [ ] Part 2 - production (coming soon)

## How to Use
- 1 git clone https://github.com/athiwatp/docker-laravel-stack.git
- 2 cd docker-laravel-stack
- 3 docker run --rm -v $(pwd):/app composer/composer install

## Setup Environment File ENV
- 1 cp .env.example .env

## Build Environment
- 1 docker-compose up
  ... wait for finish setup environment
- 2 docker-compose exec app php artisan key:generate

## For Delete and Down Container Service
- 1 docker rm (docker ps -a -q) -f
- 2 docker rmi (docker images -q)
- 3 docker network rm (docker network ls -q)
