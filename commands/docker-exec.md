# docker exec

The `docker exec` command is used to run commands inside a running Docker container. It provides a way to interact with a container, execute commands, and inspect its environment.

## Syntax

```shell
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
```

## Common Options

- **`-d` or `--detach`**: Run the command in the background.
- **`-i` or `--interactive`**: Keep STDIN open even if not attached.
- **`-t` or `--tty`**: Allocate a pseudo-TTY.
- **`--user`**: Specify the username or UID and optionally the group name or GID to use when running the command.

## Examples

1. Run a command in an interactive shell:
   ```shell
   docker exec -it my-container /bin/bash
   ```

2. Execute a single command in a running container:
   ```shell
   docker exec my-container ls -l
   ```

3. Run a command in the background:
   ```shell
   docker exec -d my-container ./my-background-script.sh
   ```

4. Specify the user for command execution:
   ```shell
   docker exec --user myuser my-container whoami
   ```

The `docker exec` command is useful for troubleshooting and debugging running containers. It allows you to interact with a container's filesystem and execute commands inside a container.