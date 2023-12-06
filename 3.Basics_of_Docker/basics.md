- It is platform that simplifies the process of building, packaging and deploying of an application in lightweight, portable containers.

### What is Cotainers?
- They are lightweight, standalone, and executable software package that includes all the dependencies required to run an application.
- Containers isolate applications from their environment, so that they work consistently across different systems.

### Main Docker Components.
- **Dockerfile** : text file containing instruction to build an docker image.
- **Docker Image** : snapshot of container, created from dockerfile.
- **Docker Container** : Running instance of docker image.

### Docker commands.
- `docker pull <image>` : It download image from registery, like docker hub.
- `docker build -t <image_name> <path>` : It build image from dockerfile, in which <path> dictates the directory containing dockerfile.
- `docker container ls` : list all running containers.
- `docker container stop <container>` : Stop a running container.
- `docker container rm <container>` : remove a stopped container.
- `dockerimage rm <image>` : remove an image from your local machine.