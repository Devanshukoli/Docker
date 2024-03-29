# What is `Docker`?

- Docker is an open-source platform for running, shipping, and developing applications. It also enables us to separate our application from the infrastructure so that we can deliver software very quickly. 
- `Docker` is open-source platform. 
	* authomates the deployment, scalling, and management of application. 
	* how it's done ? By isolating them into lightweight, portable **Containers** .
	* Now, what is *container*? 
		* Containers are standalone executalbe units that encapsulate all necessary dependencies, libraries, and config. files required for an app. to run across various environment.

# What is `container`?

- Simply put, **Container** is another process on your machine that has been isolated from all other processes on the _host machine_.

# What is this `docker platform`?
-  It provides us the ability to run an app. on an isolated environment called 'Containers'. This isolation and the security that comes within that isolated env. allows anybody to run many containers simultaneously on a given 'HOST'. 

	- These so-called 'Containers' are lightweight and contain everything needed to run the app., so we don't need to rely on what is currently installed on the host. 
		- it means,  When you run an application on a computer, it usually relies on various software components that are already installed on that computer, such as libraries, frameworks, or runtime environments. This can make it difficult to ensure that the application runs correctly on different computers with different configurations.
		- Containers, on the other hand, package the application along with all the necessary software components and configuration files, effectively creating a self-contained environment that can be run on any computer that supports container technology. This means that you don't have to worry about whether the host computer has the right software installed or not because the container has everything it needs to run the application properly. Additionally, containers are typically smaller and more lightweight than virtual machines, which can make them easier to deploy and manage.

# How Docker can be used to manage the entire lifecycle of your app., from development to deployment?

- First, you can use Docker to develop your application and all of its dependencies (such as databases, web servers, etc.) using containers. This means that everything your application needs to run is packaged together and can be easily moved between environments.

- Once you've developed and tested your application in containers, you can distribute and test it as a container. This means that you can share your application with others, and they can run it in their own environments without having to worry about setting up all the dependencies themselves.

- Finally, when you're ready to deploy your application into production, you can use Docker to either run it as a container or as an orchestrated service. This means that Docker can help you manage the deployment and scaling of your application across different environments, whether that's a local data center, a cloud provider, or a hybrid of the two.

# What can I use Dokcer for?
 
- 1. Fast, consistent delivery of your application:
	When developers use Docker, they can create local containers that include all of the software and dependencies needed to run their applications. This ensures that everyone on the development team is using the same environment, which can help eliminate bugs and compatibility issues that may arise when developers use different environments.

	- Containers are also well-suited for continuous integration and continuous delivery (CI/CD) workflows. CI/CD is a set of practices used by software development teams to build, test, and deploy code changes quickly and reliably. Using Docker containers in a CI/CD workflow can make it easier to test and deploy changes, because containers can be easily created, run, and destroyed as needed.

- 2. Respnosive deployment and scaling
	- Docker’s container-based platform allows for highly portable workloads. Docker containers can run on a developer’s local laptop, on physical or virtual machines in a data center, on cloud providers, or in a mixture of environments.

- 3. Running more workloads on the same hardware.
	- Compared to virtual machines, Docker is often faster and more lightweight, because it doesn't need to run a full operating system for each container. Instead, Docker containers share the same kernel as the host operating system, which can make them more efficient in terms of resource usage.

		- Because Docker is lightweight and efficient, it can be a cost-effective alternative to virtual machines, especially in high-density environments where many containers need to be run on a single server. Docker can allow you to use more of your server capacity to achieve your business goals, by reducing the overhead associated with virtual machines and improving the utilization of your hardware resources.

# What is the docker daemon?

- The Docker daemon is the main component of the Docker engine, responsible for managing Docker objects such as images, containers, networks, and volumes.

- When you interact with the Docker CLI (Command Line Interface) to run commands like docker run or docker build, the CLI sends requests to the Docker daemon, which then executes the requested action. The daemon is responsible for starting and stopping containers, pulling images from Docker registries, managing networks and volumes, and more.

- The Docker daemon runs as a background process on a host machine and listens for requests from the Docker CLI or other tools that interact with the Docker API. The daemon can be configured with various options, such as specifying the storage driver or setting resource limits on containers

# What is the docker client?
- The Docker client is a command-line tool that provides an interface for users to interact with the Docker daemon. The client communicates with the daemon via the Docker API, sending requests to create or manage Docker objects such as containers, images, networks, and volumes.

- When you run commands like docker run, docker builds, or docker push, you are actually interacting with the Docker client, which then sends requests to the Docker daemon to execute the requested action. The Docker client provides a simple and intuitive interface for managing Docker objects and supports a wide range of commands and options for customizing Docker behavior.

- The Docker client can be installed on any machine that needs to interact with Docker, including local development environments, build servers, or remote servers hosting production applications. In addition to the command-line interface, Docker also provides a graphical user interface (GUI) called Docker Desktop, which includes the Docker client and other tools for working with Docker.

# What is a docker registry?
-  A Docker registry is a storage and distribution system for Docker images. It allows you to store, manage, and distribute Docker images, which are the packaged application and environment components that can be used to run containers.

- The most commonly used Docker registry is the Docker Hub, which is a public registry that allows anyone to store and distribute Docker images. Docker Hub contains a vast collection of images, including official images maintained by Docker and community-contributed images.

- However, organizations can also set up their own private Docker registry to store and distribute their own Docker images internally. A private registry can be used to share images among team members or across different environments or to ensure that images are only distributed to trusted users.

- A Docker registry can be accessed using the Docker CLI or other tools that support the Docker Registry API. When you run the docker pull command to download an image, Docker will search for the image in the configured registry and download it if it's available.

# What are docker objects?
-  Docker objects are the components that make up the Docker platform and enable users to create, manage, and run containerized applications. The main Docker objects include:
	1. Images: Immutable files that contain all the instructions needed to create a container. Docker images can be stored in a Docker registry or on a local machine.
	2. Containers: Runnable instances of Docker images that can be started, stopped, and deleted as needed. Containers can be thought of as lightweight, standalone execution environments for running applications.
	3. Networks: Virtual networks that allow containers to communicate with each other and with the outside world. Docker networks can be used to isolate and secure applications running in containers.
	4. Volumes: Persistent data storage mechanisms that can be attached to containers, allowing data to persist across container restarts.
	5. Services: A way of scaling containers across multiple Docker hosts, managed by a single Docker Compose file.
	6. Swarms: A group of Docker hosts that are managed as a single entity, allowing for easy orchestration and scaling of containerized applications.


# Why do we need **Containers**?

- For that I have some blogs that will help :)
	* [first](https://cloudnativeislamabad.hashnode.dev/introduction-to-docker-part-1)
	* [second](https://cloudnativeislamabad.hashnode.dev/introduction-to-docker-part2-virtual-machines-vs-docker-containers)

- If you stuck somewhere, Just go to `Twitter or X` and search with `#docker, #container` *why we need container*. That's it.