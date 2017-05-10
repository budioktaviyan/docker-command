# Docker Command
List of Docker Command That I've learned

## Setup Machine
* Digital Ocean
`docker-machine create --driver digitalocean --digitalocean-access-token [DO_ACCESS_TOKEN] --digitalocean-image [DO_IMAGE] --digitalocean-region [DO_REGION] --digitalocean-size [DO_SIZE] [DOCKER_MACHINE_NAME]`

* Virtual Box
`docker-machine create --driver virtualbox [DOCKER_MACHINE_NAME]`

## Check Docker Environment
* List all docker environment
`docker-machine ls`

* Check specific docker environment
`docker-machine env [DOCKER_MACHINE_NAME]`

### Other Docker Command
* Access MySQL Console
`docker exec -it [CONTAINER_NAME] mysql -u root -p`

* List all docker running instance
`docker ps`

* Restart docker instance
`docker restart [CONTAINER_NAME]`

* Build docker image
`docker build --rm -t [TAG] [PATH]`

* Remove docker image
`docker rmi -f [IMAGE_ID]`

* Run docker-compose to docker instance
`docker-compose -f [DOCKER_COMPOSE_FILE] up -d`

* Run docker logs with tail
`docker logs -f --tail "[MAX_LINE]" [CONTAINER_NAME]`

* Find all unused docker images
`docker images -f "dangling=true" -q`

* Access bash into docker container
`docker exec -it [CONTAINER_NAME] bash`

* SCP zip file into docker machine
`docker-machine scp -r [ZIP_FILE] [DOCKER_MACHINE_NAME]:[PATH]`

* Check MySQL max_allowed_packet
`docker exec -it [CONTAINER_NAME] mysql -p -e "show variables like '%max_allowed_packet%';"`

### Linux Command
* Unzip file
`unzip [ZIP_FILE] -d [PATH]`
