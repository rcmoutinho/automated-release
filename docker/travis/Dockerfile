FROM ruby:alpine

RUN apk add --no-cache build-base git && \
    gem install travis && \
    gem install travis-lint && \
    apk del build-base &&\
    mkdir project

WORKDIR project
VOLUME [ "/project" ]

LABEL maintainer="twitter.com/rcmoutinho"

ENTRYPOINT [ "travis" ]