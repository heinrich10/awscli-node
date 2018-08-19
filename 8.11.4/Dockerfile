FROM node:8.11.4

RUN apt-get update && \
    apt-get upgrade -y

RUN apt-get install -y \
    python3 \
    python3-pip \
    python3-dev

ENV AWS_CLI_VERSION 1.15.81

RUN pip3 install awscli==${AWS_CLI_VERSION} && \
	rm -rf /var/lib/apt/lists/*
