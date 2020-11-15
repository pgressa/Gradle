## Push To Docker Registry Workflow
Workflow builds docker image with name `"${System.env.DOCKER_REGISTRY}/$project.name:$project.version"` and pushes the image
into configured docker registry.

The GitHub secrets in table below needs to be configured:

| Name | Description |
| ---- | ----------- |
| DOCKER_USERNAME | Docker registry username. |
| DOCKER_PASSWORD | Docker registry password. |
| DOCKER_REGISTRY | Docker image registry, for image `foo/bar:latest` it is `foo`. |
| DOCKER_REGISTRY_URL | Docker registry url. In case of using DockerHub this secret is not needed. |

> Specifics on how to configure public cloud docker registries like DockerHub, Google Container Registry (GCR), AWS Container Registry (ECR),
> Oracle Cloud Infrastructure Registry (OCIR) and many more can be found in [docker/login-action](https://github.com/docker/login-action)
> documentation.

## Feature github-workflow-docker-registry documentation

- [https://docs.github.com/en/free-pro-team@latest/actions](https://docs.github.com/en/free-pro-team@latest/actions)

## Feature http-client documentation

- [Micronaut Micronaut HTTP Client documentation](https://docs.micronaut.io/latest/guide/index.html#httpClient)

