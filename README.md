# Docker for Ruby On Rails
This repository is to create a docker in order to work on Ruby On Rails with MySQL database.

## Prerequisite
* Docker Compose (Docker For Windows or Docker For Mac, or you can use Docker-machine with Virtual Machine)

## Procedure
* Use `docker-compose up -d`
* Go inside your `ruby` container (`docker-compose exec ruby bash`), generate your app
* Configure DB to use `db` host and mysql.
* Launch your server with `rails server`
* Meet your website on docker-machine ip on 127.0.0.1

## TODO
* ~~Docker Compose 3~~
* ~~Webserver on port 80~~
* ~~No longer use Docker-machine ?~~
* Server container independant ?
* Better Readme