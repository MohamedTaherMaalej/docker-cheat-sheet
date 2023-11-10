The `docker build` command is used to build a Docker image from a Dockerfile. A Dockerfile is a text file that contains a set of instructions for creating a custom Docker image.

## Syntax

```shell
docker build [OPTIONS] PATH | URL | -
```

## Common Options

- **`-t` or `--tag`**: Name and optionally a tag in the 'name:tag' format.
- **`--build-arg`**: Set build-time variables.
- **`--file`**: Specify the path to the Dockerfile.
- **`--no-cache`**: Do not use cache when building the image.

## Examples

1. Build an image from the current directory using the default Dockerfile (Dockerfile in the current directory):
   ```shell
   docker build -t my-image:latest .
   ```

2. Specify a custom Dockerfile location:
   ```shell
   docker build -t my-app:latest -f /path/to/Dockerfile .
   ```

3. Set build-time variables:
   ```shell
   docker build -t my-app:latest --build-arg VERSION=1.0 .
   ```

4. Disable cache during the build process:
   ```shell
   docker build -t my-app:latest --no-cache .
   ```

The `docker build` command is used to create custom images tailored to your specific requirements. It is essential for building images that can be used to run containers with your application or services.