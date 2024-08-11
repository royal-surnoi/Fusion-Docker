## commands
docker pull mongo

docker -d \
-p 27017:27017 \
-e MONGO_INITDB_ROOT_USERNAME=mongoadmin \
-e MONGO_INITDB_ROOT_PASSWORD=secret \
--network 
mongo


# images build commands
docker build -t my-app:1.0