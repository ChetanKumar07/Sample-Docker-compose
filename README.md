# Sample-Docker-compose

#Docker CLI Command to run nginx app on specified port and route logs to localhost volume(without docker-compose):
docker run -d -v ~/nginxlogs:/var/log/nginx -p 5001:80 -i nginx


#Docker-compose file to run nginx app on specified port and route logs to localhost volume:
docker-compose.yml

#To run Docker Compose file:
docker-compose up -d

#For file validation:
docker-compose config

#To run Docker Compose file:
docker-compose down

#Stop and remove all docker containers:
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)

#Remove all docker images
docker rmi $(docker images -a -q)



Useful Links:
https://www.youtube.com/watch?v=Qw9zlE3t8Ko 
https://github.com/jakewright/tutorials/tree/master/docker/02-docker-compose

https://www.youtube.com/watch?v=HUpIoF_conA 
https://github.com/docker/compose/releases

https://linuxhint.com/docker_volumes_docker_compose/  
https://stackoverflow.com/questions/54374724/docker-container-save-logs-on-the-host-directory
