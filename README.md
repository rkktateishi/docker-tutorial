# Docker Tutorial

1. Setup your Docker Environment
    * [Mac](https://docs.docker.com/docker-for-mac/install/)
    * [Linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
    * [Windows](https://docs.docker.com/docker-for-windows/install/)
1. Pick your code: PhP, Python3 or dotnetcore

## Docker commands
1. `docker build . -t <image-name>` build an with a given name
1. `docker run <image-name> [options]` Run an image
1. `docker ps` View all running containers (add `-a` to view all containers)
1. `docker stop <image-name>` Stop a running image
1. `docker rm <container-name>` delete container
1. `docker rmi <image-name>` delete local image

## Docker Run Cheat sheet

Here is a list of useful arguements t o know for docker:

* `-p <host-port>:<internal-port>` Forward ports from host machine
* `-d` Run container in background
* `--name=<container-name>` Run container with a given name
* `-ti` Run container interactively
* `docker run <image-name> -ti /bin/bash` Run container with bash terminal

## Dockerfile cheat sheet

* `RUN <command>` Run a given command
* `COPY <host-path> <internal-path>` Copy files/directories from host machine to image
* `WORKDIR <internal-path>` Set working directory
* `CMD <command>` Set default command
* `FROM <image-name>` Add image layer
* `EXPOSE <port>`  Expose ports
* [Docker Documentation](https://docs.docker.com/engine/reference/builder/)
