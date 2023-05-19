FROM node:14.21.3-slim

WORKDIR /usr/src/app

RUN apt-get update && apt-get install -y --no-install-recommends git && apt-get -y clean \
    && npm init -y && npm install -g zenn-cli@latest
