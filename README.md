!/bin/bash
# Created by Elsa
# Date: Nov 2023
# Clean up ( containers and images) docker hosts server

docker rm -f $(docker ps -a -q)                                
docker rmi -f $(docker images -q)  

echo "Isn't that easy!"
