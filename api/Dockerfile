FROM ruby:2.5.7

RUN apt-get update -qq && apt-get install -y nodejs postgresql-client

WORKDIR /api

# Copy the existing Gemfile
COPY Gemfile /api
COPY Gemfile.lock /api

# Install Gems
RUN gem install bundler
RUN bundle install

COPY . /api

CMD ["rails", "server", "-b", "0.0.0.0"]