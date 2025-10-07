# CST8915 Lab 4

## Youtube Walkthrough Link

[Youtube Link](https://youtu.be/dKelAYi16bg)

## Reflection Questions

### What are the main differences between a Docker image and a Docker container?

- A docker image is a read only snapshot that contains instructions that can be used to create containers. The image contains many layers that determine different parts of the environment that will be created. A container uses an image to create an isolated environment which runs independently of the system and wont impact the system. Since containers use images to create their environment it is easy to create identical containers seperate of each other.

### Explain how Docker's layered architecture improves efficiency

- Docker's layered architecture has a few different properties which help increase it's efficiency. Docker's layers are very efficient at caching layers so that they can be reused instead of being rebuilt completely, if code in the application is changed docker will only rebuild that layer and reuse all the other layers. Docker is smart about how it stores its layers, if multiple images are downloaded with similar attributes then docker will only save one copy of each layer, for example if different images share a Ubuntu OS base layer then docker will only save one copy.

### Why does each container get its own writable layer?

- Each container getting it's own writable layer is a key part of how docker maintains it's isolation and flexibility. Since a container is created from a read-only image, each container needs a thin writable layer in order to modify files within the container. This allows docker containers to be lightweight.

### What are the benefits of using Docker Compose over running containers individually?

- Docker compose can turn multiple independent containers into one cohesive application that is easy to manage. If running multiple containers individually everything must be setup manually. In a docker compose setup everything is set up ina single yaml file, multi-container support is automatically built in, networking is configured automatically, and scaling can be achieved with a single command.
