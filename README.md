# docker-services

my private services ( webserver, database, ci etc ) on development, stage, production

### Prepare before docker contaniner up services 

```
$ docker network create -d bridge docker-services
```

### Usage

for use this services you must add to end of the file.

docker-compose.yml

```
networks:
  default:
    external:
      name: 'docker-services'
```
