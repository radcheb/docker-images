# base image is Ubuntu
FROM ubuntu:latest

MAINTAINER Radhwane Chebaane <radhwane.chebaane@eurecom.fr>

RUN apt-get update

# Install Memcached
RUN apt-get install -y memcached

# expose default port 11211
EXPOSE 11211

CMD ["/usr/bin/memcached", "-u", "memcache", "-v"]

RUN service memcached start