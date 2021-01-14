FROM ruby:2.6.0
RUN bundle config --global frozen 1
WORKDIR /usr/src/app
COPY Gemfile Gemfile.lock ./
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN bundle update --bundler
RUN gem install bundler
RUN bundle install
COPY . . 
EXPOSE 3000

RUN rails db:migrate
CMD rails s

