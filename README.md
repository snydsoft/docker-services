# dev-docker-services

my private development services ( webserver, database, ci etc )

### Prepare before docker contaniner services for development

```
$ docker network create -d bridge dev-docker-services
```

### Usage

for use this services you must append compose file on end line.

```
networks:
  default:
    external:
      name: 'dev-docker-services'
```
