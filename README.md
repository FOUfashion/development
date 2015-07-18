# Development Set-up

This is a Docker Compose app with all the services imported as submodules. It helps developers get up and running fast.

## Init

Make sure you have these installed:

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

## Run

Launch the app:

```bash
$ docker-compose up -d
```

Add these entries in `/etc/hosts`:

```
<docker-ip> docker
<docker-ip> fou.local
<docker-ip> api.fou.local
<docker-ip> rethinkdb.fou.local
```

## Extra

Also do these for your own sanity:

```bash
$ alias dk=docker
$ alias dc=docker-compose
$ alias ma=docker-machine
```
