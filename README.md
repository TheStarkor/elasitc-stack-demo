# elasitc-stack-demo

## Logstash

### Getting Started
```
$ docker pull docker.elastic.co/logstash/logstash:7.12.1
$ docker run --rm -it -v ${PWD}/pipeline/:/usr/share/logstash/pipeline/ docker.elastic.co/logstash/logstash:7.12.1 /bin/bash
$ bin/logstash -e "input { stdin { } } output { stdout { } }"
$ bin/logstash -f pipeline/*.conf
```