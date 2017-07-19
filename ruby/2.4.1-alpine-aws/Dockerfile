FROM ruby:2.4.1-alpine

RUN apk --update add build-base mysql-dev tzdata python python-dev py-pip && \
     pip install --upgrade awscli && \
     apk --purge -v del py-pip && \
     rm -rf /var/cache/apk/*
