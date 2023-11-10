# docker run

The `docker run` command is used to create and start a new container from a Docker image. It allows you to configure various aspects of the container, such as networking, volumes, and environment variables.

## Syntax

```shell
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

## Common Options

- **`-d` or `--detach`**: Run the container in the background.
- **`-it`**: Start an interactive session with a terminal.
- **`--name`**: Assign a name to the container.
- **`-p` or `--publish`**: Map container ports to host ports.
- **`-v` or `--volume`**: Mount a host directory as a volume inside the container.
- **`--env`**: Set environment variables.
- **`--network`**: Connect the container to a specific network.

## Examples

1. Run a container in the background:
   ```shell
   docker run -d nginx
   ```

2. Start an interactive session with a terminal:
   ```shell
   docker run -it ubuntu
   ```

3. Name the container:
   ```shell
   docker run --name my-container nginx
   ```

4. Publish ports and mount volumes:
   ```shell
   docker run -p 8080:80 -v /path/to/host:/path/in/container my-app
   ```

5. Set environment variables:
   ```shell
   docker run --env MYSQL_ROOT_PASSWORD=secret mysql
   ```

6. Connect the container to a specific network:
   ```shell
   docker run --network my-network my-app
   ```

The `docker run` command is highly versatile and allows you to specify various options and configurations when starting containers. Refer to the official Docker documentation for a complete list of options and their descriptions.