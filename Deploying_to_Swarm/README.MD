## Introduction
Now that we’ve demonstrated that the individual components of our application run as stand-alone containers and shown how to deploy it using Kubernetes, let’s look at how to arrange for them to be managed by Docker Swarm. Swarm provides many tools for scaling, networking, securing and maintaining your containerized applications, above and beyond the abilities of containers themselves.


In order to validate that our containerized application works well on Swarm, we’ll use Docker Desktop’s built in Swarm environment right on our development machine to deploy our application, before handing it off to run on a full Swarm cluster in production. The Swarm environment created by Docker Desktop is fully featured, meaning it has all the Swarm features your app will enjoy on a real cluster, accessible from the convenience of your development machine.


# Notes to self:


## Deploying: example used below are created with a file name bb-stack.yaml


* Deploy app to Swarm: docker stack deploy -c bb-stack.yaml demo
* list service: docker service ls
* copy and paste localhost:8000 to browser to check status
* Tear down: docker stack rm demo
