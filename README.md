# elk-cribl

a docker-compose project to run a full elk stack including cribl/logstash

## Getting Started
`docker-compose up -d --build`

after building and all containers are up and running, the services are available on your local machine

Kibana: http://localhost:5601
Elasticsearch: http://localhost:9200
Cribl: http://localhost:19000

1. Login to cribl with admin:admin and enable the in_elastic source on port 10080
2. Setup a destination to elasticsearch
3. Change the main pipeline to your created elasticsearch (not to devnull as it was preset)
4. Login to Kibana to create an index pattern named "filebeat-*"

and you should be good to go!
for more information see the documentation: https://docs.cribl.io/docs/sources-elastic
