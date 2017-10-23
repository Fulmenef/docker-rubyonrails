FROM ruby:latest

MAINTAINER Axel PERROUD <axel.perroud@outlook.com>

RUN apt-get update -qq && apt-get install -y build-essential

# for postgres
RUN apt-get install -y libpq-dev

# for nokogiri
RUN apt-get install -y libxml2-dev libxslt1-dev

# for capybara-webkit
RUN apt-get install -y libqt4-webkit libqt4-dev xvfb

# for a JS runtime
RUN apt-get install -y nodejs

# Install Rails and Bundler
RUN gem install rails bundler

# Find a way to use docker-env or something better
ENV APP_HOME /var/www/html
WORKDIR $APP_HOME

# Only if you are using existing project
#RUN bundle install