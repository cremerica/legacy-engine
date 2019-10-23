FROM openjdk:8-alpine
MAINTAINER Fernando Cremer <cremerfc@gmail.com>

ARG JARFILE
ENV JARFILE ${JARFILE}
COPY webgoat/target/$JARFILE /usr/src/webgoat/$JARFILE
WORKDIR /usr/src/webgoat
EXPOSE 8080

ENTRYPOINT java -jar $JARFILE