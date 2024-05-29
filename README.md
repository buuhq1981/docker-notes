```shell
docker image ls
docker save -o openjdk17.tar openjdk:17

docker save -o mongo-latest.tar mongo:latest
docker save -o mysql-latest.tar mysql:latest
docker save -o postgres-latest.tar postgres:latest

docker load < /tmp/mongo-latest.tar
docker load < /tmp/mysql-latest.tar
docker load < /tmp/postgres-latest.tar

rm /tmp/mongo-latest.tar
rm /tmp/mysql-latest.tar
rm /tmp/postgres-latest.tar

docker save -o mongo6-focal.tar mongo:6.0.4-focal
docker load < /tmp/mongo6-focal.tar

docker save -o postgres-14-bullseye.tar postgres:14.9-bullseye
docker load < /tmp/postgres-14-bullseye.tar
```