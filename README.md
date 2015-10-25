
# Experiment on Docker
---

> git init
> touch README.md
> mkdir -p images/api-service
> touch images/api-service/Dockerfile
> touch docker-composer.yml
> mkdir src
> cd src
> composer create-project laravel/laravel --prefer-dist
> mv laravel api-service
> cp -R api-service interface-service
> cd ..
> docker-compose up -d
> chmod -R 777 src/api-service/storage
> chmod -R 777 src/api-service/bootstrap/cache
