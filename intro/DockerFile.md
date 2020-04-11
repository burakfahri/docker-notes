# How to create Docker Images with a Dockerfile

A Dockerfile is a script that contains collections of commands and instructions that will be automatically executed
in sequence in the docker environment for building a new docker image.

Introduction to the Dockerfile Command
---
A dockerfile is a script which contains a collection of dockerfile commands and operating system commands.
Docker images contains multiple commands layer by layer. Each layer is unmodifiable. Every layer represents a command and
it is not possible to change it. 

![Docker Image Layers](https://image.slidesharecdn.com/dockerimage-150828004109-lva1-app6891/95/optimizing-docker-images-7-638.jpg?cb=1440722601 "Docker image layers")


Commands
-

* FROM
    
    The base image for building a new image. This command must be on top of the dockerfile.
    Start point of the docker file. Define the base image of the docker container.
    In the example, docker image start to build on the top of the latest version of the busybox image.
    ```
    FROM busybox:latest
    ```
    
* RUN
    
  Used to execute a command during the build process of the docker image.
  ```
  RUN cat env
  ```
  
* ADD

  Copy a file from the host machine to the new docker image. There is an option to use a URL for the file,
  docker will then download that file to the destination directory.
  Adds files and folders to the docker container.
  ```
  ADD folder {specific_directory}
  ```  

* ENV
  
  Define an environment variable.
  Example to define java home environment variable of the docker container
  ```
  ENV JAVA_HOME={java_home_directory}
  ```

* CMD
  
  Used for executing commands when we build a new container from the docker image.
  Example to run app.py
  ```
  CMD ["python", "./app.py"] 
  ```
* ENTRYPOINT
  
  Define the default command that will be executed when the container is running.
  It generally place at the bottom of the dockerfile.
  In this example, entry point is the first process of the container while running.
  ```
  ENTRYPOINT java -cp /apps/myapp/myapp.jar com.jenkov.myapp.Main
  ```
* EXPOSE
  Exposes the ports of the docker image to outside of the world.
  Example to expose 80 and 8080 to the host machine
  ```
  EXPOSE 80 8080
  ```
