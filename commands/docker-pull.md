# docker pull

The `docker pull` command is used to download Docker images from a specified container registry, such as Docker Hub. This command is helpful when you want to fetch Docker images that you intend to use or run on your local system.

## Syntax

```shell
docker pull [OPTIONS] NAME[:TAG|@DIGEST]
```

Common Options
--all-tags: Pull all available image tags for the given repository.
--disable-content-trust: Skip image signature verification.
-a or --arch: Specify the architecture for the image.
--platform: Set the platform for which to pull the image.

Examples
Pull a specific image from Docker Hub:

```shell
docker pull ubuntu:20.04
```

Pull all available tags for a repository:

```shell
docker pull --all-tags nginx
```
Disable content trust and skip image signature verification:

```shell
docker pull --disable-content-trust my-image
```

Pull an image for a specific architecture:

```shell
docker pull -a arm64v8/ubuntu:20.04
```

Specify the platform for image pulling:

```shell
docker pull --platform linux/amd64 my-image
```

The docker pull command allows you to retrieve Docker images from remote registries and store them locally. You can then use these images to run containers on your local system. It's a fundamental step in the process of working with containers.