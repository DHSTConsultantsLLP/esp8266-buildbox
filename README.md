# esp8266-buildbox
Dockerfile for esp8266-buildbox on Ubuntu 14.04
make sure the devicemapper is selected instead of ausfs in /etc/default/docker.io
Use DOCKER_OPTS to modify the daemon startup options like this:
DOCKER_OPTS="--storage-driver=devicemapper"
