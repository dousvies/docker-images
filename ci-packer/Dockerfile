FROM alpine:3.8

ARG PACKER_VERSION=1.7.0
ENV PACKER_VERSION $PACKER_VERSION

RUN apk add curl ansible git jq

RUN curl -L "https://releases.hashicorp.com/packer/${PACKER_VERSION}/packer_${PACKER_VERSION}_linux_amd64.zip" -o ./packer.zip

RUN unzip packer.zip && rm -f packer.zip && chmod +x packer && \
    mv ./packer /usr/local/bin/packer

RUN rm -rf /var/cache/apk/* && \
    rm -rf /var/tmp/*