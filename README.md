```sh
docker run -d --name postgresql_tst -e POSTGRESQL_PASSWORD=123456 -e POSTGRESQL_USERNAME=postgres -e POSTGRESQL_DATABASE=test -p 35432:5432 bitnami/postgresql:latest

docker run -d --name mongodb_tst -e MONGODB_USERNAME=mongo -e MONGODB_PASSWORD=123456 -e MONGODB_DATABASE=test -p 47017:27017 bitnami/mongodb:latest

docker run -d --name redis_tst -e REDIS_PASSWORD=123456 -p 56379:6379 bitnami/redis:latest

yarn
yarn typeorm migration:run
yarn dev:server
```
