* Lists various properties of running containers.
```
docker ps
```
* Lists various properties of all containers.
```
docker ps -a

#alternative way
docker ps --all
```
* Runs a command in a container that is active or running.
```
docker exec -i {running_container_id} {command}

example to connect to terminal of running container: 
    docker exec -it {running container id} sh
```
* Starts already stopped containers.
```
    docker start {container_id}
``` 
* Stops already stopped containers.
```
    docker stop {container_id}
``` 
* Remove containers.
```
#if the container already stoped
docker rm {container_id}

#if the container runs, you need to stop it or delete it forcely
docker rm -f {container_id}
``` 

* Stops and starts a container.
```
docker restart {container_id}
``` 

* Runs a command in an isolated container.
```
docker run {docker_image}
```

For all commands: [docker container commands link](https://docs.docker.com/engine/reference/commandline/container/)
