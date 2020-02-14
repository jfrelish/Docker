## Introduction.


Now that we’ve demonstrated that the individual components of our application run as stand-alone containers, it’s time to arrange for them to be managed by an orchestrator like Kubernetes. Kubernetes provides many tools for scaling, networking, securing and maintaining your containerized applications, above and beyond the abilities of containers themselves.


In order to validate that our containerized application works well on Kubernetes, we’ll use Docker Desktop’s built in Kubernetes environment right on our development machine to deploy our application, before handing it off to run on a full Kubernetes cluster in production. The Kubernetes environment created by Docker Desktop is fully featured, meaning it has all the Kubernetes features your app will enjoy on a real cluster, accessible from the convenience of your development machine.


## Notes: 


* Deployment-describing a scalable group of identical pods.
* NodePort- service, which will route traffic from port 30001 on your host to port 8080 inside the pods it routes to, allowing you to reach your bulletin board from the network.


## Deploying *example below is using a bb.yaml file created through text editor*

* kubectl apply -f bb.yaml
* Make sure everying works by listing: kubectl get deployments
* Open browser and paste localhost:30001 



[moreinfo](https://docs.docker.com/get-started/part3/)






