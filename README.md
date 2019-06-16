docker volume create mongo-volume
docker run --name mongo -v mongo-volume:/data/db -p 27017:27017 -d mongo --auth
docker exec -it mongo mongo admin