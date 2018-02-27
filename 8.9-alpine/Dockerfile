FROM node:8.9.4-alpine

# Versions: https://pypi.python.org/pypi/awscli#downloads
# from https://raw.githubusercontent.com/sekka1/aws-cli-docker/master/Dockerfile
ENV AWS_CLI_VERSION 1.14.47

RUN apk --no-cache update && \
    apk --no-cache add python py-pip py-setuptools ca-certificates groff less && \
    pip --no-cache-dir install awscli==${AWS_CLI_VERSION} && \
    rm -rf /var/cache/apk/*
