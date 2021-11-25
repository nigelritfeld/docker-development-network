# Environment for local development 
This repo contains files for setting up a local development environment using docker.
The environment contains the following tech stack:
- MariaDB
- MyPhpAdmin
- Nginx
- PHP 8

## Install docker desktop
To use this repo you need docker engine with docker compose installed.

Refrence the docker website to install docker engine on you machine.
https://www.docker.com/products/docker-desktop

## Get started

Navigate to the repo and create te following folder:

    $ mkdir data
    $ cd data
    $ mkdir mariadb

Next to start the environment run:

    $ docker-compose run -d

Goodluck! 🍀
