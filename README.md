!/bin/bash
# Created by Elsa
# Date: Nov 2023
# Clean up ( containers and images) docker hosts server

docker rm -f $(docker ps -a -q)   ## delete all containers                              
docker rmi -f $(docker images -q)  # delete all images

echo "Isn't that easy!"