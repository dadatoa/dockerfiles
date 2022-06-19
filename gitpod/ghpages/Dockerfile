FROM ruby

RUN gem install --force bundler
RUN gem install jekyll webrick rouge
RUN gem install github-pages

WORKDIR /srv/jekyll
VOLUME  /srv/jekyll
EXPOSE 35729
EXPOSE 4000