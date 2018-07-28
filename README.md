## Elasticsearch + Kibana Docker Compose file

This project contains a docker-compose.yml file that creates an elasticsearch 2 node
cluster and a Kibana conected to that cluster.

#### Prerequisites
For this to work on your machine you need to install:
- Git
- Docker (latest versions of Docker already ship with docker-compose)

#### Run Elasticsearch + Kibana
Clone this repo:
```
git clone https://github.com/lombritz/elastic-kibana-docker.git
cd elastic-kibana-docker
```
And run:
```
docker-compose up -d
```
After a few minutes click [here](http://localhost:5601) to enter Kibana.

Thats it!

#### Trouble Shooting

TBD
