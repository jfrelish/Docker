
























Introduction
Now that we’ve got our orchestrator of choice set up in our development environment thanks to Docker Desktop, we can begin to develop containerized applications. In general, the development workflow looks like this:
Create and test individual containers for each component of your application by first creating Docker images.
Assemble your containers and supporting infrastructure into a complete application, expressed either as a Docker stack file or in Kubernetes YAML.
Test, share and deploy your complete containerized application.
