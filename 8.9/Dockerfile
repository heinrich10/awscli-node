FROM node:8.9

RUN apt-get update && \
    apt-get upgrade -y

RUN apt-get install -y \
    python \
    python-pip \
    python-dev

ENV AWS_CLI_VERSION 1.14.47

RUN pip install awscli==${AWS_CLI_VERSION} && \
	rm -rf /var/lib/apt/lists/*
