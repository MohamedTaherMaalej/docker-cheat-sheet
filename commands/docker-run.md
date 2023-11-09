# docker run

The `docker run` command is used to create and start a new container from a Docker image. It allows you to configure various aspects of the container, such as networking, volumes, and environment variables.

## Syntax

```shell
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```
Common Options
-d or --detach: Run the container in the background.
-it: Start an interactive session with a terminal.
--name: Assign a name to the container.
-p or --publish: Map container ports to host ports.
-v or --volume: Mount a host directory as a volume inside the container.
--env: Set environment variables.
--network: Connect the container to a specific network.


Examples
Run a container in the background:
```shell
docker run -d nginx
```
Start an interactive session with a terminal:
```shell
docker run -it ubuntu
```
Name the container:
```shell
docker run --name my-container nginx
```
Publish ports and mount volumes:
```shell
docker run -p 8080:80 -v /path/to/host:/path/in/container my-app
```
Set environment variables:
```shell
docker run --env MYSQL_ROOT_PASSWORD=secret mysql
```
Connect the container to a specific network:
```shell
docker run --network my-network my-app
```