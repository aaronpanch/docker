FROM circleci/ruby:2.4.1-node

RUN sudo apt-get update && sudo apt-get -y install python-pip libpython-dev
RUN pip install --upgrade --user awscli \
  && echo "export PATH=~/.local/bin:$PATH" > ~/.bashrc
