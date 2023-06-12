FROM bash:alpine3.15

RUN apk add --no-cache jq findutils && \
    curl -fsSL git.io/aria2c.sh | bash && \
    rm -rf /var/cache/apk/* /tmp/*
    
RUN apk add --no-cache parallel
COPY . /docker
RUN chmod +x /docker/download.sh
ENTRYPOINT ["/docker/download.sh"]
