# Traefik and Nginx in Docker for Ubuntu 20.04
## How to prepare and getting started
### Installation of necessary software
1. `apt update`
2. `apt install docker.io -y`
3. `sudo curl -SL https://github.com/docker/compose/releases/download/v2.24.6/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose`
4. `sudo chmod +x /usr/local/bin/docker-compose`
### Getting started
1. `git clone https://github.com/Xopco/traefik.git` into the directory which you plan to run the project
2. `docker network create proxynet`
3. `docker-compose up -d`

