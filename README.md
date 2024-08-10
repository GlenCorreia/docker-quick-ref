# Docker Notes 🐳

### <u>Docker Images vs Containers</u>
A package or artifact that we produce with Docker is called a **Docker Image**.

- **Definition**: A Docker image is a lightweight, standalone, and executable software package that includes everything needed to run a piece of software—code, runtime, libraries, environment variables, and configuration files.
- **Static**: An image is a read-only template. It’s a blueprint or a snapshot of an application and its environment.
- **Creation**: Docker images are built from a Dockerfile, which defines the steps to assemble the image, like installing software packages, setting environment variables, etc.
- **Layers**: Docker images are composed of multiple layers, where each layer represents a change or addition to the image. Layers are reusable across different images, making the images lightweight.

A **Docker Container** is a running instance of a Docker Image.

- **Definition**: A Docker container is a running instance of a Docker image. It’s a virtualized runtime environment that is isolated from the host system and other containers.
- **Dynamic**: Containers are mutable. Once a container is created, it can be started, stopped, moved, or deleted.
- **Execution**: Containers are the active entities that perform the actual work. When you run a Docker image, you create a container.
- **Isolation**: Containers provide an isolated environment for the application, with their own file system, networking, and process space.


In summary, Images are the blueprints or templates used to create containers. They are static and read-only. Containers are the instances of images. They are dynamic, running, and can be modified while running.

You can run multiple containers from 1 image.

Run the following command in terminal to get the list of all images that are there on your Docker. <br>
`$ docker images`

Run the following command to get a list of containers. <br>
`$ docker ps`

### <u>Docker Registries</u>



