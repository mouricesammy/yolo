## Backend And Client Base Images
 node:19-alpine - Alpine  is much smaller than most distribution base images hence creates small image sizes

## DB
  mongo : for mongo DB

## Dockerfile commands/instructions 

 FROM : specifies parent image for docker 
 WORKDIR : sets working directory for any docker commands run. i.e docker RUN,COPY etc
 RUN : executes commands during the image build time
 COPY: copies new files or directories from <src> and adds them to the filesystem of the container at the 
    path <dest> 
 EXPOSE : specifies docker listening ports
 CMD :provides  default initialization command that is executed once a container is created from the Docker image

## Docker-compose Networks

contains frontend and backend tier networks for isolation, security and communication between both layers using different ips/networks.
the networks are as follows:
 frontend
  networks:
      front-end-network:
        ipv4_address: 172.127.0.3
 backend
  networks:
      front-end-network:
        ipv4_address: 172.127.0.2
      backend-end-network:
        ipv4_address: 172.128.0.2
  

## Docker Hub

This images runs successfully, pull their images from docker hub link below and test.
 [Docker-Hub] (https://hub.docker.com/search?q=mourice)