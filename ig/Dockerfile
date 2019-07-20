FROM ruby:2.4.6
RUN apt-get update -qq && apt-get install -y nodejs postgresql-client
RUN mkdir /opt/app
COPY . /opt/app/
WORKDIR /opt/app/
RUN bundle install