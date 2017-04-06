# Docker Command
List of Docker Command That I've learned

## SETUP MACHINE
* Digital Ocean
`docker-machine create --driver digitalocean --digitalocean-access-token [DO_ACCESS_TOKEN] --digitalocean-image [DO_IMAGE] --digitalocean-region [DO_REGION] --digitalocean-size [DO_SIZE] [DOCKER_MACHINE_NAME]`

* Virtual Box
`docker-machine create --driver virtualbox [DOCKER_MACHINE_NAME]`

## Check docker environment
* List all docker environment
`docker-machine ls`

* Check specific docker environment
`docker-machine env [DOCKER_MACHINE_NAME]`

## Access MySQL Console
`docker exec -it [DOCKER_INSTANCE] mysql -u root -p`

### Other docker command
* List all docker running instance
`docker ps`

* Restart docker instance
`docker restart [DOCKER_INSTANCE]`

* Build docker image
`docker build -t [TAG] [PATH]`

* Remove docker image
`docker rmi -f [IMAGE_ID]`

* Run docker-compose to docker instance
`docker-compose -f [DOCKER_COMPOSE_FILE] up -d`
