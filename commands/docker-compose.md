# docker-compose

The `docker-compose` command is used to define and run multi-container Docker applications. It allows you to manage complex containerized applications by specifying services, networks, and volumes in a `docker-compose.yml` file.

## Syntax

```shell
docker-compose [OPTIONS] COMMAND [ARGS...]
```

## Common Commands

- **`up`**: Create and start containers based on the `docker-compose.yml` file.
- **`down`**: Stop and remove containers, networks, and volumes defined in the `docker-compose.yml` file.
- **`build`**: Build or rebuild services.
- **`ps`**: List containers.
- **`logs`**: View output from containers.
- **`exec`**: Run a command in a running container.
- **`pull`**: Pull service images.
- **`restart`**: Restart services.
- **`down`**: Stop and remove containers, networks, and volumes.
- **`config`**: Validate and view the compose file.

## Examples

1. Start containers defined in the `docker-compose.yml` file:
   ```shell
   docker-compose up
   ```

2. Build or rebuild services:
   ```shell
   docker-compose build
   ```

3. View logs from services:
   ```shell
   docker-compose logs
   ```

4. Run a command in a running container:
   ```shell
   docker-compose exec service_name command
   ```

5. Stop and remove containers, networks, and volumes:
   ```shell
   docker-compose down
   ```

6. Restart services:
   ```shell
   docker-compose restart
   ```

The `docker-compose` command simplifies the management of multi-container Docker applications. It relies on a `docker-compose.yml` file to define the application's services, networks, and volumes. Refer to the official Docker Compose documentation for more details and advanced usage.