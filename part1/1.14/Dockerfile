FROM ruby:2.6.0

EXPOSE 3000

RUN apt -y update && apt -y upgrade
RUN apt -y install git nodejs
RUN git clone https://github.com/docker-hy/rails-example-project
WORKDIR rails-example-project
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD ["rails", "s"]
