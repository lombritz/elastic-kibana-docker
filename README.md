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

To check if it started successfully run:
```
user$ docker ps --format "{{.ID}} : {{.Image}}" | grep kibana
889b778b5817 : docker.elastic.co/kibana/kibana:6.3.2
```
Replacing the actual container_id run:
```
docker logs -f 889b778b5817
```
This will follow the Kibana container logs, you'll know when its ready when you see this line:
```
{"type":"log","@timestamp":"2018-07-28T15:39:03Z","tags":["listening","info"],"pid":1,"message":"Server running at http://kibana.local:5601"}
```
Thats it!

#### Trouble Shooting

TBD
