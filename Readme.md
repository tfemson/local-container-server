# Local Server Containers

A shared container for micro services. This resource servers (db, redis, rabbitmq, etc.), are meant for local development purposes only. 

The objective is driven by concepts of abstraction, resource sharing, and separation of concerns, by having a separate docker project whose purpose is to encapsulate resource containers that other projects can connect to, without having to spin up their own containers for databases and the likes. Thus having more lightweight docker setups for individual projects, and a more appropriate setup for integrated local development across multiple projects.

## Prerequisites

- Docker

1. Start the containers:
    ```shell
    $ docker compose up
    ```
   To check that the container is running, open a terminal window/tab and run `docker ps` to see info about the
   currently running docker containers. Any or all of the following container names (depending on the ones you choose to run) should be listed among the running containers:
    - `local-postgres`
    - `local-mariadb`
    - `local-mysql`
    - `local-redis`
    - `local-rabbit`