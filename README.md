# Development Set-up

This is a Docker Compose app with all the services imported as submodules. It helps developers get up and running fast.

## Get started

Make sure you have these intalled:

```bash
$ git -v
$ docker -v
$ docker-compose -v
```
Clone this repo and install dependencies:

```bash
$ git clone git@github.com/FOUfashion/development.git Fou && cd Fou
$ git submodule init && git submodule update
$ git submodule foreach npm install
```

Launch the app:

```bash
$ docker-compose up -d
```

Also do these for your own sanity:

```bash
$ alias dk=docker
$ alias dc=docker-compose
$ alias ma=docker-machine
```

## Env vars

```bash
export NODE_ENV=development
export PORT=3000
export HOSTNAME=localhost
export RETHINKDB_HOST=docker
export RETHINKDB_PORT=28015
export RETHINKDB_DB=test
export CLI_ENABLED=true
export CLI_PORT=4000
```
