# https://www.elastic.co/guide/en/logstash/current/docker-config.html

FROM docker.elastic.co/logstash/logstash-oss:7.16.2

RUN bin/logstash-plugin install logstash-output-s3

ADD logstash.conf /usr/share/logstash/pipeline/logstash.conf
ADD jvm.options /usr/share/logstash/config/
ADD start.sh /usr/share/logstash/bin/start.sh
