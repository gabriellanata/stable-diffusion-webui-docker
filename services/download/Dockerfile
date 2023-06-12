FROM bash:alpine3.15

RUN apk add --no-cache aria2
RUN apk add --no-cache parallel
COPY . /docker
RUN chmod +x /docker/download.sh
ENTRYPOINT ["/docker/download.sh"]
