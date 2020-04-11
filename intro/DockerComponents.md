# Docker components
![Docker Components](https://docs.docker.com/engine/images/architecture.svg "Docker components")
---

### Docker Engine

It is the core part of the whole Docker system. 
Docker Engine is an application which follows client-server architecture. Docker engine allows all the images run 
in several different OS with the same behaviour.

It is installed on the host machine. There are three components in the Docker Engine:

* Server: It is the docker daemon called dockerd. It can create and manage docker images.
* Rest API: It is used to instruct docker daemon what to do.
* Command Line Interface (CLI): It is a client which is used to enter docker commands.
---

### Docker daemon
The Docker daemon (dockerd) listens for Docker API requests
and manages Docker objects such as images, containers, networks, and volumes.
A daemon can also communicate with other daemons to manage Docker services.

---

### Docker Client

Docker users can interact with Docker through a client. When any docker commands runs,
the client sends them to dockerd daemon, which carries them out.
Docker API is used by Docker commands. Docker client can communicate with more than one daemon.
---

### Docker Registries

It is the location where the Docker images are stored. It can be a public docker registry or a private docker registry.
Docker Hub is the default place of docker images, its stores’ public registry.
 You can also create and run your own private registry.

When you execute docker pull or docker run commands, the required docker image is pulled from the configured registry.
When you execute docker push command, the docker image is stored on the configured registry.
---

### Docker Objects

Docker objects are :
* Images
* Containers
* Volumes
* Networks

For the detailed information you can use the [next](./DockerObjects.md)
