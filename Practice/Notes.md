## Introduction
	Containers are lightweight, portable, and isolated software environments that allow developers to run and package applications with their dependencies, consistently across different platforms.




---------------------------------------------
Container vs Image
Versions and Tags
Docker Commands
	- Docker pull
	- Docker images
	- Docker run
	- Docker start
	- Docker stop
	- Docker ps
	- docker logs
	- docker exec -it
- Container is a running environment for a Image which combines of (application Image + environment configuration + file system)
- Docker run = pull + start
- docker run <image_name>:<tag>

- Container Port vs Host Port

Host Port        | 5000    |  3000   | 3001          
--------------------------------------------
Contaner Ports   | 5000    |  3000   | 3000

same host will get confilicts so that , we can avoid by giving different port

>> docker run  <container_name> -p <Host_port>:<container_port>
docker run redis -p 6379:6379 
docker run redis:4.7 -p 6000:6379
--------------------------------------
docker logs 
-d detach mode
-p port mapping
-e env variables

--name:<name_for_container>
docker exec
-it interactive terminal  
>> docker exec -it <container_id> /bin/bash
here we can do any kind of operatops 

-----------------------------------------
Docker provides default networks
>> docker network ls 

to create network 
>> docker network create mongo-network 
--net <network_name>
------------------------------------------
docker compose

volumes for data consistence 

Docker volume location (linux-ubuntu)
/var/lib/docker/volumes
