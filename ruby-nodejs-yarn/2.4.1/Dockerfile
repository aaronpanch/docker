FROM ruby:2.4.1

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -

# Previous command runs update
RUN apt-get install -y build-essential nodejs

RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - \
  && echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list

RUN apt-get update && apt-get install -qy yarn

CMD [ "irb" ]
