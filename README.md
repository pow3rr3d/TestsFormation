# SF5DockerInstall


This repository is a personnal ready-to-use repository for [Symfony 5](https://symfony.com/) using [WSL2](https://docs.microsoft.com/fr-fr/windows/wsl/install-win10) and [Docker](https://www.docker.com/products/docker-desktop) interface.

## Bashrc
In order to simplify the use of docker, please enter the following line in your bashrc (sudo nano ~/.bashrc):
* alias dc='docker-compose --env-file .env $*'
* alias php='docker-compose -f ../docker/docker-compose.yml exec php-fpm php $*'
* alias composer='docker-compose -f ../docker/docker-compose.yml exec php-fpm composer $*'

## Composer

Start to make: 

* cd < project dir>/src
* composer update

If you need to use composer like "composer require ...", you must be in the < project dir>/src .

## Npm

Start to make: 

* cd < project dir>/src
* npm install

If you need to use composer like "npm install ...", you must be in the < project dir>/src .

## Docker
To start Docker, please make:

* cd < project dir>/docker
* dc up -d

To start Docker, please make:
* dc down

## Contributing

Pull request are welcome.
