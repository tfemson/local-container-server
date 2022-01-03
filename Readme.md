# Local Server Containers

A shared container for micro services. This resource servers (db, redis, rabbitmq, etc.), are meant for local development purposes only. 

The objective is driven by concepts of abstraction, resource sharing, and separation of concerns, by having a separate docker project whose purpose is to encapsulate resource containers that other projects can connect to, without having to spin up their own containers for databases and the likes. Thus having more lightweight docker setups for individual projects, and a more appropriate setup for integrated local development across multiple projects.

## Prerequisites

- Docker