FROM docker.elastic.co/beats/filebeat:7.14.0

# Support and Update for this Dockerfile
LABEL Maintainer="s.bechstein@gmail.com" 

COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN chown -R root:filebeat /usr/share/filebeat/

USER filebeat