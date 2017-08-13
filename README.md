# RestAPIPractice Practice

### Download docker-tool first
* Mac: https://docs.docker.com/docker-for-mac/
* Windows: https://docs.docker.com/docker-for-windows/

### How to start the app
```sh
docker-compose up 
```
### How to rebuild the app
```sh
docker-compose down #stop the current running app
docker-compose rm -f #remove existing container
docker-compose up --build -d #Build the app and bring it up
```

### How to check the app's stdout in docker instance

* First check the docker container id by running
```sh
docker ps [--all]
```
* Then check the log by running
```sh
docker logs -f <app_container_id>
```
### How to stop and remove docker container
* Get all containers
```sh
docker ps --all
```
* Stop and kill container by names
```sh
docker stop <NAMES>
docker rm <NAMES>
```

### Yelp Search API query example
https://gist.github.com/yschen5812/e5ef56c3d14aa224c72114f20cd8115f
