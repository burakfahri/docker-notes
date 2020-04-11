* Build an image from a Dockerfile
```
docker image build	
```

* Pull an image from docker hub. If you don't specify any repository, it will automatically try to pull image from  [docker hub](https://hub.docker.com).
For example to fetch the mysql latest image, you can use 
you can got more detailed information from the [link](https://hub.docker.com/_/mysql)
```
docker pull {image_id}
```

* List all the images
```
docker image ls
```

* To remove an image 
```
    docker rmi -f {image_id/image_tag}
``` 

* Display detailed information on one or more images
```
    docker image inspect {image_id/tag}
``` 

* Remove unused images.
```
docker image prune
``` 

* Push an image to one of the docker repository
```
docker push {container_id/tag}
``` 

* To tag an image
```
docker image tag  {new_image_name:new_image_version}
```

For all commands: [docker image commands link](https://docs.docker.com/engine/reference/commandline/image/)
