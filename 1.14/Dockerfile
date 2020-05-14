FROM ruby:2.6.0

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs

WORKDIR /usr/src/myapp
COPY . /usr/src/myapp

RUN gem install bundler
RUN bundle install
RUN rails db:migrate

CMD rails s