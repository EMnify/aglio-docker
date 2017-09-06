# Aglio in Docker

Dockerfile for [emnify/aglio](https://hub.docker.com/r/emnify/aglio/).

## Usage

Just prepend your `agilo` command with

    docker run -it -v $PWD:/docs -w /docs emnify/aglio:latest

This will use the `latest` tag of the container and mount the current working directory as volume into the Docker at `/docs`.

It is recommended to specify the _Aglio_ version, whic are available as [tags](https://hub.docker.com/r/emnify/aglio/tags/), e.g., `emnify/aglio:2.2.1`.

If a new version of _Aglio_ is not yet available, just edit the `Dockerfile` and push it to a branch matching the version number. This will trigger an automated build of the Docker image.

