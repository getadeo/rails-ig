FROM ruby:2.4.3
RUN apt-get update -qq && apt-get install -y nodejs postgresql-client
RUN mkdir /opt/app
COPY Gemfile /opt/app/Gemfile
COPY Gemfile.lock /opt/app/Gemfile.lock
COPY . /opt/app/
WORKDIR /opt/app/
RUN bundle install