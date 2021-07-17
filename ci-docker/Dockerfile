FROM docker:20.10

RUN apk add --no-cache curl git jq python3 python3-dev py-pip && \
    pip install awscli --quiet --no-cache && \
    rm -rf /var/cache/apk/* && \
    rm -rf /var/tmp/*
