1. docker is a open-source platform that automate the deployment and scalling in your application using the containerise technology.
   is called Docker.

2. Docker file is a script that contain the instrustion for building the docker images.

3. Docker images is a read only binaray template that contain the instrustion for creating a docker container.

4. container hold the entire package that need to run your application inlcude runtime system tool, system libraries we can call is like 
virtual machine.

5. Docker hub is a cloud based respoity service. that allow to users upload and download your images private and public environment.

6. Docker Networking.

  1. Bridge Network - container are connected to by default bridge network can communicate with each other, bridge network get in own private ip
  addresss like 172.16.0.0/17. Inside the bridge network there are two types. 

     1. Default - it is automatic crreate when docker is installed. but DNS is not supporting 
     2. Custom - it is manually created by user it offer more flexible and better isolation compare to default network. but DNS
        is supported 

  2. Host Network- the container share the host network stack no isolation between container and host network. 

  3. Overlay- it is Designed for docker swarm connecting to multiple docker deamon to enable the docker communication between 
     docker swarm.

  4. Mac Vlan - it is assigend the mac address to a each containers.

  5. None- the container has no network idealy when you want complete isolation between container and host network.


7. RUN- it is used to execute the cmd during the build -processs install package and dependencies
   
   CMD- is a a default cmd to run when the container is started.
   
   Entrypoint- it is used to specific and fixed command that always run when container is started, any additional arguments 
   passed to the container will be passed to the entrypoint.    

8. COPY- is a used to copy the files and directory from the build content into the image. 

   ADD- it is used to file transfer with extra feature. when you want download the files from url and extract the tar acrived 


9. Container runtime is a software component responsible for running containers on the host system.
It is used to start, stop, and manage containers 

10. Docker Engine is the core software that enables you to build, run, and manage containers on a host machine.

11. is a tool used to define run multi-container of Docker applications. It allows you to manage multiple Docker containers using a single YAML configuration file (docker-compose.yml)

12. A Docker Volume is a persistent storage  used  by Docker containers to store and share data. volumes data is aviable even after the container is removed or restarted.

13. The Docker Daemon is the background service that:  (dockerd) Manages all Docker containers, images, networks, and volumes

14. A multi-stage build is Docker uses the  multiple FROM statements in one Dockerfile to separate the build environment from the final runtime environment. It helps create smaller, 
    cleaner, and more secure images by copying only the necessary build artifacts from the builder stage into the final image.


15.  init container- Run before the main application containes. Always run before app containers. Wait for a database to be ready.
     
     Side Car-  Runs alongside the main application container

     Ephemeral Container- Used for debugging a running Pod, Troubleshoot the pod and debugging

16. 1. Alpine- is a very small and ligtwigt image compare to other images used to create smaller, faster, and more secure containers.

    2. Slim Image - A slim image is a minimal version of a base image, containing only  runtime components. 
    It removes unnecessary files like documentation, package managers, libaries, and debugging tools

    3. Distroless Image - You don’t need debugging tools inside the container, No package manager, no shell, no OS tools — contains only your app + its dependencies.

    
