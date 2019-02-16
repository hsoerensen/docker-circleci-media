FROM circleci/ruby:2.6.1-node

RUN echo "deb http://ftp.uk.debian.org/debian jessie-backports main" | sudo tee -a /etc/apt/sources.list && sudo apt-get update -qq
RUN sudo apt-get purge graphicsmagick graphicsmagick-dbg imagemagick-common graphicsmagick-libmagick-dev-compat -y && sudo apt-get autoremove -y && sudo apt-get install ffmpeg imagemagick libmagickwand-dev -y
RUN sudo apt-get update -qq && sudo apt-get install -y mysql-client openjdk-8-jdk openjdk-8-jre