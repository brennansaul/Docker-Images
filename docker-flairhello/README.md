# FlairHello

## Overview
Dockerized Hello World image for dsplaying load balancing.

- Operating System: Alpine 
- Base Image: [ resin/raspberry-pi-alpine-node](https://hub.docker.com/r/resin/raspberry-pi-alpine-node/) 

## Files

- `Dockerfile`
- `index.php`
- `logo.png`
- `run.sh`
- `php-fpm.conf`
- `docker-cloud.yml`
- `docker-compose.yml`
- `nginx.conf`
- `README.md`

## Exposed ports

- 80 

## Volumes 

- n/a

## Environment Variables 

- LISTEN_PORT=80

## How to use from the Docker CLI

1. Make sure that Docker CLI is running 
2. Start container `docker run -d -p 2500:80 brennansaul/flairhello`
3. In your browser navigate to `localhost:2500`

## Instructions for building and running image on your own computer

1. Clone this repository 
2. Navigate on you local machine to the directory containing the Dockerfile 
3. Build command: `docker build -t falirhello .`
4. Run command: `docker run -d -p 2500:80 falirhello`
5. In your browser navigate to `localhost:2500`

