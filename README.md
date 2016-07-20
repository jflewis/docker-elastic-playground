# Docker Elastic Playground

## Use cases 
The general use case for this is to test logstash configurations for log 
aggregation into elasticsearch

All you would have to do here is add your application image under the app service
in the docker-compose.yml

## Configuration files
The default configuration assumes that ...

1. Your logstash conf file is in the logstash directory
1. Your app uses a .env file and that file is located in the app directory 

### Notes
You will have to expose container and host ports on the logstash service
for whichever ports you have logstash listening on

This was only tested on Docker 1.11> so I can not make any promises that it will work on a older version