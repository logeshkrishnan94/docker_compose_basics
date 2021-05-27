# Docker Compose Basics

A basic [Docker Compose](https://docs.docker.com/compose/) template for orchestrating a [Flask](http://flask.pocoo.org/) application & a [Celery](http://www.celeryproject.org/) queue with [Redis](https://redis.io/)

### Clone repo

```bash
git clone https://github.com/logeshkrishnan94/docker_compose_basics
```

### Build & Launch

```bash
docker-compose -f docker-compose.yml up --build
```

### Only Launch

```bash
docker-compose -f docker-compose.yml up
```

This will expose the Flask application's endpoints on port `5001` as well as a [Flower](https://github.com/mher/flower) server for monitoring workers on port `5555`


To shut down:

```bash
docker-compose down
```
