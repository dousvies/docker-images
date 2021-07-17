FROM python:3.8-slim

RUN apt-get -qq update && \
    apt-get -y -qq dist-upgrade && \
    apt-get -qq install -y python3-dev python3-pip ca-certificates groff less bash make jq curl wget g++ zip git gettext && \
    pip install -q --no-cache awscli && \
    apt-get -qq clean