# docker container for gitbucket

This docker container of [gitbucket](https://github.com/gitbucket/gitbucket.git) is under testing!!!

## usage

### dependencies
- [docker](https://docs.docker.com/engine/installation/)
- [docker-compose](https://docs.docker.com/compose/install/)

### installation

1. Get code from repository:
```
git clone https://gitbucket.pgollor.de/git/docker/gitbucket.git
cd gitbucket
```

2. Generate new passwords for your databse!!!
```
./generate_password.sh
```

3. Change the confoguration and start with:
```
docker-compose up -d
```

4. Open `127.0.0.1:8080` and be habby. :-)


### configuration
Please use the configuration file `gitbucket.conf` for your personal changes.
There are three configs for gitbucket:
- `GITBUCKET_BIND`: ip address to bind to
- `GITBUCKET_WEB_PORT`: web port to bind to
- `GITBUCKET_SSH_PORT`: ssh port to bind to


## Inspirations
I got some inspirations for this project from:
- https://github.com/mailcow/mailcow-dockerized

