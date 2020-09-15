FROM ruby:2.6.0
EXPOSE 3000
ADD rails-example-project .
RUN apt-get update
RUN apt install --allow-unauthenticated -y nodejs
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD rails s