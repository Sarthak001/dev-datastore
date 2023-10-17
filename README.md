# Datastore
Database containers for your all development needs.
Datastore quickly configures and deploy database instances according to your needs.

## Features
Database users and password can be configured in the dockercompose.yml itself

- [Mariadb] - maraidb instance @ localhost:3306

- [adminer] - adminer instance for easy management of maraidb @ localhost:8082

- [mongodb] - mongodb instance @ localhost:27017

- [mongo-express] - mongo-express for easy management of mongdb @ localhost:8081

## Deployment

```sh

cd datastore
sudo docker-compose up -d

```

## Reset Specfic DataStore

If something went wrong, We can reset that particular Database.

```sh

sudo docker-compose down
sudo docker ps -a
sudo docker rm -f <CONTAINER_ID_OF_DATABASE_YOU_WANT_TO_RESET>
sudo docker volume ls -q
sudo docker volume rm <VOLUME_ID_OF_DATABASE>
sudo docker-compose up -d

```