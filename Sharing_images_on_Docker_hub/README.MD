# Introduction


At this point, you’ve built a containerized application in Part 2, and potentially run it on Kubernetes in Part 3 or Swarm in Part 4, all on your local development machine thanks to Docker Desktop. The final step in developing a containerized application is to share your images on a registry like Docker Hub, so they can be easily downloaded and run on any destination cluster.


## Notes: 

* Setup a [docker hub account](https://hub.docker.com/signup)
* On Docker Toolbar sign in with your created docker hub account. 

## Push to dockerHub

* Click docker icon, Repositories, create and it will take you to the Docker hub page
* Fill out repository name, then create
* docker name formatting example: *<Docker Hub ID>/<Repository Name>:<tag>; ex. docker image tag bulletinboard:1.0 gordon/bulletinboard:1.0*
* Push to Docker Hub ex: docker image push gordon/bulletinboard:1.0.
* It should now be on the docker hub page. 

