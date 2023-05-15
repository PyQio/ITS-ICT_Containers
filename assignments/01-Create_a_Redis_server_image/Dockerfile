FROM ubuntu:latest
USER root   
RUN apt update && apt install -y redis-server
EXPOSE 6380/tcp

USER redis
COPY ./redis.conf /etc/redis/redis.conf 
LABEL maintainer = "Simone Pugliese" 
ENTRYPOINT ["redis-server", "/etc/redis/redis.conf"]
