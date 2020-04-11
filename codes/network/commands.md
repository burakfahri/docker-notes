* List networks
```
docker network ls 
```
* Connect a container to a network
```
docker network connect {image_id} {network_id}
```
* Create a network
```
docker network create [options]
```

* Disconnect a container from a network
```
docker network disconnect
```

* Display detailed information on one or more networks
```
docker network inspect {network_id}
``` 

* Remove all unused networks
```
docker network prune
``` 

* Remove one or more networks
```
docker network rm {network_id}
``` 
For all commands: [docker network commands link](https://docs.docker.com/engine/reference/commandline/network/)
