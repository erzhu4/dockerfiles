FROM ubuntu:latest as ubuntu-env

RUN apt-get update -y && apt-get install -y openssl zip unzip git && apt-get install -y vim && apt-get install -y curl && apt-get install -y nginx

RUN echo "My php7.2 with nginx dockerfile"