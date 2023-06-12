FROM bash:alpine3.15

RUN apk add --update aria2
RUN apk add --update parallel
COPY . /docker
RUN chmod +x /docker/download.sh
ENTRYPOINT ["/docker/download.sh"]
