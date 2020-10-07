FROM ruby:2.7-alpine
RUN apk add --no-cache build-base gcc bash cmake git
RUN gem install bundler jekyll
WORKDIR /sitedagabriela
COPY . /sitedagabriela/
RUN bundle install
CMD ["bundle", "exec", "jekyll", "serve", "-H", "0.0.0.0"]
