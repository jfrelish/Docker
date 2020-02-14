

## Introduction
Now that we’ve got our orchestrator of choice set up in our development environment thanks to Docker Desktop, we can begin to develop containerized applications. In general, the development workflow looks like this:
Create and test individual containers for each component of your application by first creating Docker images.
Assemble your containers and supporting infrastructure into a complete application, expressed either as a Docker stack file or in Kubernetes YAML.
Test, share and deploy your complete containerized application.


## Windows:



Step 1 After installing Docker Desktop, you should see a Docker icon in your system tray. Right-click on it, and navigate Settings -> Kubernetes.


step 2 Check the checkbox labeled Enable Kubernetes, and click Apply. Docker Desktop will automatically set up Kubernetes for you. Note this can take a significant amount of time (20 minutes). You’ll know everything has completed successfully once you can right-click on the Docker icon in the menu bar, click Settings, and see a green light beside ‘Kubernetes is running’.


step 3 n order to confirm that Kubernetes is up and running, create a text file called pod.yaml with the following content:


step 4 In powershell, navigate to where you created pod.yaml and create your pod:
 

 kubectl apply -f pod.yaml

 

 step 5 Check that your pod is up and running:
 

 kubectl get pods


Step 6 Check that you get the logs you’d expect for a ping process:
 

 kubectl logs demo


Step 7 Tear down test pod commant: kubectl delete -f pod.yaml


## Swarm 

Step 1 Initialize docker swarm on power shell: docker swarm init


Step 2 Run a simple Docker service that uses an alpine-based filesystem, and isolates a ping to 8.8.8.8:
 

 docker service create --name demo alpine:3.5 ping 8.8.8.8


Step 3 Check to see if a container is running: docker service ps demo


Step 4 Check logs: docker service logs demo


Step 5: Tear down: docker service rm demo



My notes: When installing Docker, All previous Docker including docker toolbox must be deleted, an error will appear when attempting to run Docker terminal. 
