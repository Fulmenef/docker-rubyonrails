# Docker for Ruby On Rails
This repository is to create a docker in order to work on Ruby On Rails with MySQL database.

## Prerequisite
* Docker Machine
* Virtual Machine
* Docker Compose

## Procedure
* Create a docker-machine
* Use `docker-compose up -d`
* Go inside your `ruby` container, generate your app 
* Configure DB to use `db` host.
* Launch your server with `rails server`
* Meet your website on docker-machine ip on port 3000

## TODO
* Docker Compose 3
* Webserver on port 80
* No longer use Docker-machine ?
* Server container independant ?
* Better Readme