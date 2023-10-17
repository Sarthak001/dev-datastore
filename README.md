# Datastore
Database containers for your all development needs.

Datastore quickly configures and deploy database instances according to your needs.



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