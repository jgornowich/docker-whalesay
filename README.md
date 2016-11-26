# Cowsay Project with Docker

This is a slightly modified version of the Docker getting started reference that guides you through building your own images [here](https://docs.docker.com/engine/getstarted/step_four/).

[Docker page] (https://hub.docker.com/r/jgornowich/docker-whalesay/)

# Usage
 
```bash
# Build the container
$ docker build -t jgornowich/docker-whalesay .

# Run the container 
$ docker run --rm jgornowich/docker-whalesay cowsay hello

# Run the container with a different cow
$ docker run --rm jgornowich/docker-whalesay cowsay -f tux hello
$ docker run --rm jgornowich/docker-whalesay cowsay -f devil hello
$ docker run --rm jgornowich/docker-whalesay cowsay -f calvin "Where is hobbes?"
$ docker run --rm jgornowich/docker-whalesay cowsay -f ghostbusters "I aint afraid of no ghost"

# Enter the container to see what is there
$ docker run --rm -ti --entrypoint /bin/bash jgornowich/docker-whalesay
```
