Scaling microservices using Kubernetes and Docker

## Key terms
* Microservices
* 12 Factor Rules (Or guidelines) for developing good and reliable applications
* JWT - JSON Web Tokens 
* Docker
  * Why do we even need Docker?
  * Our OSs do a terrible job in running multiple instances or multiple versions of the same application without much headache initially, so we use Docker.

### Docker Installation
* To install 
` sudo apt-get install docker.io `

* To view the available images
`sudo docker images`

* To pull NGINX and all its dependencies (as a Docker image of course)
`sudo docker pull nginx:1.10.0`

* to run a container
`sudo docker run <instance_name>`
or in our case
`sudo docker run -d nginx:1.10.0`

* To view the various Docker instances
`sudo docker ps`

* to view more info about a container
`sudo docker inspect <container_id>`

* to clean up instances
`sudo docker stop <container_id>`

* to remove docker instances form the system entirely
`sudo docker rm <container_id>`

~If we specify a docker image which is not present in our local system, then Docker actually pulls it from the docker server and then runs it for us~
~Smart boy Docker!~


