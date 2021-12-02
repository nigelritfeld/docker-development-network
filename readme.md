# Environment for local PHP development 
This repo contains files for setting up a local development environment using docker.
The environment contains the following tech stack:
- MariaDB
- MyPhpAdmin
- Nginx
- PHP 8
- Xdebug

## Install docker desktop
To use this repo you need docker engine with docker compose installed.

Refrence the docker website to install docker engine on you machine.
https://www.docker.com/products/docker-desktop

## Get started

1. Navigate to the repo and open a terminal then execute this command:


```shell script
 $ mkdir data/
       cd data/
       mkdir mariadb/
       cd ..
```
### Running the environment
2. Next to start the environment run:
```
    $ docker-compose up --build
```

3. Place your projects and files in the "project folders"


4. In the browser navigate to: http://localhost/

### Stopping the environment

You can easily stop the environment by opening docker desktop interface and stopping the network, or you can execute the following command:
```
    $ docker-compose down
```  

## PhpMyAdmin

PhpMyAdmin is available on http://localhost:8080

* The Host is 'mariadb' wich will resolve to the correct ip adress in the docker network *

When you are using PHP to connect to your local database use the following credentials

| Credentials        | values        |
| ------------------ |:-------------:|
| Host               | mariadb       |
| User               | root          |
| Password           | my-secret-pw  |

## Contact

This development environment is meant for php development.
Let me know if you have any feedback! 

Goodluck! 🍀
