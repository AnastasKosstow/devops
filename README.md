
* [Docker](#Docker)
  * [Commands](#essential-docker-commands)
  * [Dockerfile](#dockerfile)
  * [Example](#end-to-end-example)

# Docker
### What is Docker?
Docker is a containerization platform that allows to put applications and their dependencies into isolated, lightweight containers.
<br>
These containers can run consistently across different environments, such as development, testing, and production, ensuring that an application behaves the same way regardless of the underlying infrastructure.

Docker containers work by running on top of the Docker Engine, which uses the host operating system's kernel but allows each container to be isolated, manage its own dependencies, and execute independently.

### Key Docker Concepts:
 - **Images**: Docker images are the building blocks of containers. They contain everything needed to run an application, including the code, runtime, system tools, and libraries.
 - **Containers**: Containers are instances of Docker images. They run in isolated environments and provide a consistent runtime environment for applications.
 - **Docker Hub**: Docker Hub is a repository for finding and sharing Docker images.

## Essential Docker Commands
 - `docker build` Build an image from a Dockerfile
 - `docker run` Create and run a new container from an image
 - `docker ps` List containers
 - `docker start` Start one or more stopped containers
 - `docker stop` Stop one or more running containers
 - `docker rm` Remove one or more containers
 - `docker rmi` Remove one or more images
 - `docker image` Manage images
 - `docker images` Lists all images stored locally
 - `docker pull` Downloads an image or a repository from a registry
 - `docker push` Uploads an image or a repository to a registry
 - `docker login` Authenticates to a Docker registry
 - `docker logout` Logs out from a Docker registry.
 - `docker exec` Runs a command in a running container
 - `docker logs` Fetches the logs of a container
 - `docker network` Manages networks
 - `docker volume` Manages volumes. Volumes are used to persist data generated by and used by Docker containers

---
 
 ### `docker build`
 Builds a Docker image from a Dockerfile. A Dockerfile contains a set of instructions for creating an image that includes the application, its dependencies, and runtime environments.

 `docker build [OPTIONS] PATH | URL`
  - `PATH` specifies the location of the Dockerfile and related context (e.g., files used in the build).
  - `URL` can be used to specify a Git repository as the source of the Dockerfile and context.
  - **Optional parameters**
    - `-t`, `--tag`: Name and optionally a tag in the 'name:tag' format
    - `--build-arg` Set build-time variables
    - `--no-cache` Do not use cache when building the image.
    - `-f, --file` Name of the Dockerfile (Default is PATH/Dockerfile).

**Examples:**
 - `docker build -t {image name} -f Dockerfile .` - build image with name
 - `docker build -t {image name}:{tag} --no-cache --build-arg {arguments like - ENVIRONMENT=production} -f Dockerfile .` - build image with name, arguments and no cache during building

---

### `docker run`
 Creates a new container from a specified image and starts it. If the image is not available locally, Docker will attempt to pull it from the configured registry.

 `docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`
  - `IMAGE` is the name of the image to start the container from.
  - `COMMAND` and ARG specify the command to run inside the container.
  - **Optional parameters**
    - `-d, --detach` Run container in background and print container ID.
    - `--name` Assign a custom name to the container. If not specified, Docker generates a random name.
    - `-p, --publish` Publish a container's port(s) to the host. Format: hostPort:containerPort.
    - `-e, --env` Set environment variables. Format: VARIABLE=value.
    - `--rm` Automatically remove the container when it exits. This is useful for not leaving behind any stopped containers.
    - `-v, --volume` Mount a volume. Format: hostSrc:containerDest or just the volume name if using Docker volumes.

**Examples:**
 - `docker run --name {container name} {image name}` - start a container from an image
 - `docker run -d --name {container name} {image name}` - start a container in the background
 - `docker run -e ENVIRONMENT=production --name {container name} {image name}` - start a container with an environment variable

---

 ### `docker ps`
 Lists containers. By default, it shows only running containers.

`docker ps [OPTIONS]`

**Optional parameters**
 - `-a, --all`: Show all containers (default shows just running).
 - `-q, --quiet`: Only display container IDs.
 - `-f, --filter`: Filter the output based on conditions like status, id, name, etc.

**Examples:**
 - `docker ps` - List running containers.
 - `docker ps -a` - List all containers, including those that are stopped.
 - `docker ps -q` - List the IDs of all running containers.

---

### `docker start`
Starts one or more containers.

`docker start [OPTIONS] CONTAINER [CONTAINER...]`

- **CONTAINER**: The container ID or name. You can specify multiple containers to start.

**Optional parameters**
 - `-a, --attach`: Attach STDOUT/STDERR and forward signals.
 - `-i, --interactive`: Attach container's STDIN.

**Examples:**
 - `docker start {container name or ID}` - Start a stopped container.
 - `docker start -a {container name or ID}` - Start a stopped container and attach to it.

---

### `docker stop`
Stops one or more running containers.

`docker stop [OPTIONS] CONTAINER [CONTAINER...]`

- **CONTAINER**: The container ID or name. You can specify multiple containers to stop.

**Examples:**
- `docker stop {container name or ID}` - Stop a running container.
- `docker stop $(docker ps -q)` - Stop all running containers by passing the IDs of all running containers.

---

### `docker rm`
Removes one or more containers.

`docker rm [OPTIONS] CONTAINER [CONTAINER...]`

- **Optional parameters**
 - `-f, --force`: Force the removal of a running container (uses SIGKILL).
 - `-v, --volumes`: Remove the associated volumes with the container.

**Examples:**
 - `docker rm {container name or ID}` - Remove a stopped container.
 - `docker rm -f $(docker ps -a -q)` - Forcefully remove all containers, including running ones.

---

### `docker rmi`
Removes one or more images from the local storage. This command is used to manage the disk space by cleaning up unused images.

`docker rmi [OPTIONS] IMAGE [IMAGE...]`

- **IMAGE**: The image ID, repository, or tag. You can specify multiple images to remove.

**Optional parameters**
- `-f, --force`: Force removal of the image, even if it's being used by stopped containers or has dependent child images.
- `--no-prune`: Do not remove untagged parents.

**Examples:**
- `docker rmi {image ID or repository:tag}` - Remove a specific image by its ID or name and tag.
- `docker rmi -f {image ID}` - Forcefully remove an image, even if it is being used.
- `docker rmi $(docker images -q)` - Remove all images by passing the IDs of all images.

---

### `docker image`
Manages images. This is a parent command for several subcommands used to manage images in Docker.

`docker image [COMMAND]`

Some common subcommands include:
- `ls`: List images.
- `rm`: Remove one or more images.
- `pull`: Pull an image or a repository from a registry.
- `push`: Push an image or a repository to a registry.
- `build`: Build an image from a Dockerfile.

Each subcommand has its own set of options and usage.

**Examples:**
- `docker image ls` - List all images.
- `docker image rm {image ID or name:tag}` - Remove a specific image.
- `docker image pull {repository:tag}` - Pull an image from a registry.
- `docker image push {repository:tag}` - Push an image to a registry.

---

### `docker images`
Lists all locally stored Docker images. This command provides a quick way to see what images are available on your system.

`docker images [OPTIONS] [REPOSITORY[:TAG]]`

- **Optional parameters**
  - `-a, --all`: Show all images (default hides intermediate images).
  - `-q, --quiet`: Only show image IDs.
  - `--format`: Pretty-print images using a Go template.
  - `-f, --filter`: Filter output based on conditions provided.

**Examples:**
- `docker images` - List all top-level images, their repository, tag, ID, creation time, and size.
- `docker images -a` - List all images, including intermediate images.
- `docker images -q` - List the IDs of all images.
- `docker images --format "{{.Repository}}:{{.Tag}} {{.Size}}"` - List images with a custom format showing repository, tag, and size.
- `docker images -f "dangling=true"` - List all dangling images (images without tags).

---


## Dockerfile
In summary, this Dockerfile defines a multi-stage build process where the first stage builds the .NET application, and the second stage prepares a lighter runtime environment to run the application.

```dockerfile
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env
WORKDIR /App

COPY . ./

RUN dotnet restore

RUN dotnet publish -c Release -o out

FROM mcr.microsoft.com/dotnet/aspnet:8.0
WORKDIR /App
COPY --from=build-env /App/out .
ENTRYPOINT ["dotnet", "{service name}.dll"]
```

`FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env` - This line is telling Docker to use the .NET SDK version 8.0 image from Microsoft's Container Registry as the base image for the build process.
  - `Container Registry` - Storage for container images. In the context of this file: It is Microsoft's own container registry designed to provide a globally available service for pulling Microsoft's container images.
  - `AS build-env` - Set a name to this stage to use it later like a variable.

`WORKDIR /App` - Sets the working directory inside the container to /App. This is the directory where your application's code will reside within the container during the build process.

`COPY . ./` - Copies everything from your project's folder (where the Dockerfile is located) into the current working directory inside the container (*/App*).

`RUN dotnet restore` - Executes the dotnet restore command. This command looks at the .NET project files in the container and downloads any dependencies (*libraries and packages*) that are needed to build the project.

`RUN dotnet publish -c Release -o out` - This command builds your .NET application in release mode (*optimized for production*) and outputs the compiled files to the *out* directory within the */App* directory in the container.
 - `-c Release` - The -c Release option specifies that the build should be done in Release configuration, which is optimized for performance.

`FROM mcr.microsoft.com/dotnet/aspnet:8.0` - After building the application, this line starts a new stage in the Dockerfile. It uses the .NET runtime image (*not the SDK*) version 8.0 as the base image. This image is lighter than the SDK image and is suitable for running the application but not for building it.

`WORKDIR /App` - Sets the working directory in this new stage (runtime stage) to */App*, similar to what was done in the build stage.

`COPY --from=build-env /App/out .` - Copies the compiled application from the out directory of the build-env (*the first stage*) to the current working directory (*/App*) of the current stage. This means we are transferring only the necessary files needed to run the application, leaving behind the source code, SDK, and any other unnecessary files.

`ENTRYPOINT ["dotnet", "{service name}.dll"]` - Specifies the command to run when the container starts. This is the main assembly that was compiled and published in the previous steps.


# End-to-end example

**Create a Dockerfile**
```dockerfile
# Use the .NET 8 SDK image to build the application
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env
WORKDIR /App

# Copy csproj and restore any dependencies (via NuGet)
COPY *.csproj ./
RUN dotnet restore

# Copy the project files and build the application
COPY . ./
RUN dotnet publish -c Release -o out

# Use the .NET 8 runtime image to run the application
FROM mcr.microsoft.com/dotnet/aspnet:8.0
WORKDIR /App
COPY --from=build-env /App/out .
ENTRYPOINT ["dotnet", "MyApp.dll"]
```

This Dockerfile does the following:
 - Starts with the .NET 8 SDK image to build your application.
 - Sets the working directory to /App.
 - Copies the .csproj file and restores dependencies.
 - Copies the application's source code and publishes the application to the out directory.
 - For the final image, it switches to the .NET 8 runtime image.
 - Copies the published application from the build environment to the runtime environment.
 - Specifies the command to run the application.

**Build the Docker Image** - `docker build -t my-dotnet-image .`

**Run the Container** - `docker run -d -p 8080:80 --name my-dotnet-container my-dotnet-image`

**View the Container's Logs** - `docker logs my-dotnet-container`