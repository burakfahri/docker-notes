#HELLO WORLD EXAMPLE
In this example, we will pull one basic image which is hello-world from the docker hub
create a container from this image and run it.

Firstly, it is needed to be sure to have a setup of the docker client in your local. Run
```
docker --version
```
in your local and output should like to be following:
```
Docker version 19.03.5, build 633a0ea
```

To pull the latest hello-world, run the following command:
```
docker pull hello-world
```

Run ```docker image ls``` command to see the image in the list.

After running the command in the terminal, docker will automatically pull the latest version of the [hello-world image](https://hub.docker.com/_/hello-world).
If you run the image with ```docker run hello-world --name hello-world-container``` command, a container which is attached to process of the terminal.
To detach the container from the terminal, add -d to the command. ```docker run -d hello-world --name hello-world-container```.

Using ```docker ps```, docker containers can be listed and see the container information on the terminal.

Using ```docker exec -it hello-world-container bash```, it is possible to connect to terminal of the container.
The command mean is execute the bash command of the container and return the output.

Exit the terminal with ```exit``` command to return to host terminal.

It is possible to see the details of the container and image also with the following command:
```
docker inspect hello-world-container
docker image inspect hello-world
```

remove the container:
```
docker rm -f hello-world-container
```

remove the image:
```
docker rmi -f hello-world
```

