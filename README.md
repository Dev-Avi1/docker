What is Docker?
Docker is an open platform designed to help developers build, ship, and run applications inside containers. Containers are lightweight, isolated environments that package all the dependencies and code your application needs to run, ensuring it works consistently across different environments.
Isolation and Security: Containers provide a secure and isolated environment, allowing multiple containers to run on the same host without interfering with each other

Portability: Docker containers can run on any infrastructure, whether it's a developer's laptop, a data center, or a cloud provider.

Efficiency: Containers are more lightweight compared to traditional virtual machines, as they share the host operating system's kernel.

Consistency: Docker ensures that your application runs the same way in development, testing, and production environments, reducing the "it works on my machine" problem.

DEPLOYMENT
==========
Deployment refers to the process of making a software system available for use. This involves several activities, including:

Release: Preparing the software for distribution.

Installation: Setting up the software on the target systems.

Activation: Making the software operational.

Deactivation: Temporarily stopping the software.

Uninstallation: Removing the software from the system.

Update: Applying new versions or patches to the software.

Version Tracking: Keeping track of different versions of the software12.

Deployment can be complex due to the diverse and unpredictable nature of target systems. Modern practices like continuous delivery and deployment automation help streamline this process1.

Install your application (jar/war)
Configure the application (db/certificates)
Starting the applications

Containerization
=================
Containerization is a method of packaging software code along with all its dependencies, libraries, and configuration files into a single, lightweight executable unit called a container. This container can run consistently across different computing environments.

Portability: Containers can run on any infrastructure, whether it's a developer's laptop, a data center, or a cloud provider.

Efficiency: Containers share the host operating system's kernel, making them more lightweight and faster to start compared to traditional virtual machines.

Isolation: Each container runs in its own isolated environment, ensuring that applications do not interfere with each other.

Scalability: Containers can be easily scaled up or down to handle varying loads, making them ideal for modern cloud-native applications.


DOCKER 
=========
IMAGE MANAGEMENT
Image management refers to the process of organizing, storing, and accessing digital images in an efficient and systematic manner. It involves several key tasks
1- Categorization
2- metadata assignment
3- Serching and Retrival
4- Storage

CONTAINER MANAGEMENT 
Container management is the process of organizing, deploying, scaling, and maintaining containerized applications across various environments. It involves several key activities:
1- Container Orchestartion
2- Monitoring and Logging
3- Secrity
4- Resource allocation
5- Updating and patching


Commands to install the Docker into the linux machine
$ sudo su 
$ apt update
$ apt install -y docker.io
$ systemctl status docker | systemctl start docker 
$ docker info
$ sudo usermod -a -G docker ubuntu 


DOCKER COMMANDS 
$ docker run --name <Cname> - it -d -p <HP>:<CP> -v <HD>:<CD> <image> <StratupCMD>
> Download the image from registry 
> Create a new container, uniue ID 
> Start the container execute the startup cmd 
> attach to the container interactively

$ docker images
$ docker ps 
$ docker ps -a
$ docker start <CID/Cname>
$ docker stop <CID/Cname>
$ docker rm <CID/Cname>
$ docker attach <CID/Cname>
$ docker logs <CID/Cname>
$ docker logs -f <CID/Cname>
$ docker exec <CID/Cname> <cmd>
$ docker exec -it <CID/Cname> <cmd>


