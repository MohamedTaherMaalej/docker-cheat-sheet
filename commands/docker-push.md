# docker push

The `docker push` command is used to push a Docker image to a specified container registry. After building and tagging your image, you can use this command to upload the image to a registry, making it accessible to others.

## Syntax

```shell
docker push [OPTIONS] NAME[:TAG]
```

Common Options

--disable-content-trust: Skip image signature verification.

--all-tags: Push all tagged images.

Examples
Push an image to Docker Hub:

docker push my-username/my-image:latest
Skip content trust and push the image:

```shell
docker push --disable-content-trust my-registry/my-image:latest
```

Push all tagged images for a repository:

```shell
docker push --all-tags my-registry/my-image
```

The docker push command is crucial when you want to share your Docker images with others by uploading them to a container registry. Ensure you have the necessary permissions to push images to the specified registry.
