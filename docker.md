# 1. Remove unused networks:
docker network prune

# 2. Remove Docker network:
docker network ls
docker network rm network_name

# 3. Remove all Docker images:
docker image rm $(docker images)