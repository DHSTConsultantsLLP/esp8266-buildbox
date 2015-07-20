# esp8266-buildbox
Dockerfile for esp8266-buildbox on Ubuntu 14.04
make sure the devicemapper is selected instead of ausfs in /etc/default/docker.io
Use DOCKER_OPTS to modify the daemon startup options like this:
DOCKER_OPTS="--storage-driver=devicemapper"
I had issue of my 8 core cpu shutting down due to overheating in compilation task i had to change the cpufreq tools to use powersave profile like this sudo cpupower frequency-set -g powersave
