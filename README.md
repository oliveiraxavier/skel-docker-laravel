# skel-docker-laravel

No arquivo .env substituir DB_HOST=127.0.0.1 para DB_HOST=db  para estar de acordo com:

services > db


Pausar containers 
docker stop $(docker ps -aq)

Listar containers 
docker ps 

Executar um container

docker exec -it <container-ID> bash


Subir um container
docker-compose up -d --build

Subir um container, recriando
docker-compose up -d --force-recreate --remove-orphans

Remover um ou mais containers
docker rm $(docker images -q)

Remover uma ou mais imagens
docker rmi $(docker images -q)
