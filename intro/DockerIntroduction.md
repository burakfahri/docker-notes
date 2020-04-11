# Docker overview

Docker is an open platform for developing, shipping, and running applications.
Docker enables you to separate your applications from your infrastructure so you can deliver software quickly.
With Docker, you can manage your infrastructure in the same ways you manage your applications. 


# The Docker platform
Docker provides the ability to package and run an application in a loosely isolated environment called a container.
The isolation and security allow you to run many containers simultaneously on a given host.

***Containers are lightweight because they don’t need the extra load of a hypervisor, 
but run directly within the host machine’s kernel.***

![dockerVsVm](https://geekflare.com/wp-content/uploads/2019/09/traditional-vs-new-gen.png "Docker vs VM")

VMs work on the hypervisor. It isolates the whole virtual machines from the main hosts but the docker containers work on
the top of the docker engine so they share the same host and directly use the os itself.

* What’s the Diff: 

| *VMs*  | *Containers*
| ------------- |:-------------:
| Heavyweight      | Lightweight
| Limited performance     | Native performance      
| Each VM runs in its own OS | All containers share the host OS  
| Allocates required memory | Requires less memory space  
| Each VM runs in its own OS | All containers share the host OS  
| Fully isolated and hence more secure | Process-level isolation, possibly less secure  

see the [next](./DockerComponents.md)

