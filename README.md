# docker-tutorial

1. [Introduction](#introduction)
2. [Common commands](#common-commands)
3. [Docker file](#docker-file)
4. [Docker page](./tutorials/docker.md)


## Introduction

<p>
Instruction of docker. How to handle with images, containers and docker file.
</p>

## Common commands

- **docker images** - list of images
- **docker ps** - list running containers\
    -a - list of running and stopped containers
- **docker pull {IMAGENAME}:{VERSION}** - download image from docker hub\
  IMAGENAME:latest - download latest with tag latest
- **docker run {IMAGENAME}:{VERSION}** - run image\
    -d or --detach - run container in background\
    -p or --publish {HOST_PORT}:{DOCKER_PORT}- bind port from docker inner port to outside port\
    --name - give name for container
- **docker stop {CONTAINER ID} or {NAME}** - terminate container with id
- **docker start {CONTAINER ID} or {NAME}** - start created container again 
- **docker logs {CONTAINER ID} or {NAME}** - get container logs
- **docker build**\
    -t or --tag - sets name and optional tag name:tag
- **docker exec -t -i {CONTAINER ID} or {NAME} /bin/sh** - runs sh in container\
  --detach , -d 		Detached mode: run command in the background\
  --detach-keys 		Override the key sequence for detaching a container\
  --env , -e 		Set environment variables\
  --env-file 		Read in a file of environment variables\
  --interactive , -i 		Keep STDIN open even if not attached\
  --privileged 		Give extended privileges to the command\
  --tty , -t 		Allocate a pseudo-TTY\
  --user , -u 		Username or UID (format: <name|uid>[:<group|gid>])\
  --workdir , -w 		Working directory inside the container

## Docker file
<p><i>Text document that contains commands to assemble an image </i></p>

- **\#** - comments
- **FROM** — build this image from the specific image
    FROM node:19-alpine
- **LABEL** — describes metadata. Fоr example an author.
- **ENV** — mont static environment.
- **RUN** — executes command in a shell inside container environment
    RUN npm install
- **COPY** — copy files or directories from \<src> and adds them to the filesystem of the container at the path \<dest>\
    COPY \<src> \<dest>\
    COPY package.json /app/
- **ADD** — copies files and directories in container. Can unpack .tar.
- **CMD** — the instruction that is to be executed when a docker container starts. There can be only one CMD instruction in a docker file
- **WORKDIR** — sets working directory for all following commands
- **ARG** — mount environment for docker when image is assembling.
- **ENTRYPOINT** — show command with arguments for calling in running container.
- **EXPOSE** — sets local port
    {HOST_PORT}:{DOCKER_PORT}
- **VOLUME** — point to mount with current vault
