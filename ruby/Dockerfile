FROM ruby:latest

MAINTAINER Axel PERROUD <axel.perroud@outlook.com>

ARG app_home

RUN apt-get update -qq && apt-get install -y build-essential

# for postgres
RUN apt-get install -y libpq-dev

# for nokogiri
RUN apt-get install -y libxml2-dev libxslt1-dev

# for capybara-webkit
RUN apt-get install -y libqtwebkit4 libqt4-dev xvfb

# for a JS runtime
RUN apt-get install -y nodejs

# Install Rails and Bundler
RUN gem install rails bundler

WORKDIR $app_home

# Only if you are using existing project
#RUN bundle install