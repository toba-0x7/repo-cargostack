## Containerization Project using Docker
## Prerequisites:
- Ubuntu 2204 VM
- docker-engine
## Objectives:
- Install Ubuntu 2204 VM
- Install docker-engine
- Add dockerfiles
- Create docker images 
- Upload images to dockerhub
## Ubuntu 22014 VM Installation
https://github.com/toba-0x7/notebook/blob/main/os-linux/setup.md
## Docker-engine Installation
https://github.com/toba-0x7/notebook/blob/main/containerization-docker/setup.md
## Add dockerfiles
- Create docker files for app, database & web\
The Dockerfile in the app directory sets up a multi-stage build to build a Java web application using Maven and then deploys it to a Tomcat server.\
The Dockerfile in the db directory sets up a MySQL database container and imports a SQL backup file during initialization\
The Dockerfile in the web directory sets up an Nginx web server container and customizes its configuration by replacing the default configuration file
- Create the nginvproapp.conf\
The configuration as seen in nginvproapp.conf represents an Nginx server block that acts as a reverse proxy to forward requests to an upstream server named vproapp.
- Create the docker-compose.yml file\
The created docker-compose.yml file is a multi-container setup for the vProfile application, including a database, cache server, message queue, application server, and web server.
## Create docker images
run in the working directory
```
docker-compose up -d
```
## Upload Images
https://docs.docker.com/get-started/04_sharing_app/
