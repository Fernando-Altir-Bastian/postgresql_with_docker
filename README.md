![Logo of the project](./Logo.png)

## Docking Postgres

Docking the PostgreSQL database


## Technology 

Here are the technologies used in this project.

* Docker version 20.10.5, build 55c4c88 (https://www.docker.com/)
* PostgreSQL version 9.6.7 Alpine (Docker Image: https://hub.docker.com/_/postgres/)


## Services Used

* Dockerhub (https://hub.docker.com/)


## Getting started

* To start, you need to have docker installed (Docker Engine overview: https://docs.docker.com/engine/)

## How to use

* Create network to access container PostgreSQL:
>   $ docker network create --driver bridge name_network

* To dockerize the PostgreSQL run:
>    $ docker run --name local-postgres9.6.7 -p 5432:5432 -e POSTGRES_PASSWORD=enter_the_postgres_password --network=name_network --mount type=bind,source=$PWD,target=/var/lib/postgresql/data postgres:9.6.7-alpine

* To run the PostgreSQL:
>    $ docker start local-postgres9.6.7

## Versioning of this project 

1.0.0.0


## Authors

* **Fernando Altir Bastian**: https://github.com/Fernando-Altir-Bastian
