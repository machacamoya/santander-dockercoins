# santander-dockercoins
```
sudo docker image build --file hasher/Dockerfile --tag index.docker.io/machacamoya/santander-dockercoins:test-hasher hasher/
sudo docker image build --file rng/Dockerfile --tag index.docker.io/machacamoya/santander-dockercoins:test-rng rng/
sudo docker image build --file webui/Dockerfile --tag index.docker.io/machacamoya/santander-dockercoins:test-webui webui/
sudo docker image build --file worker/Dockerfile --tag index.docker.io/machacamoya/santander-dockercoins:test-worker worker/
sudo docker network create hasher-network
sudo docker network create redis-network
sudo docker network create rng-network
sudo docker volume create redis-volume
sudo docker container run --detach --name redis --network redis-network --volume redis-volume:/


