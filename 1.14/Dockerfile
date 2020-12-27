# rails backend
FROM ruby:2.6.0

WORKDIR /usr/app

RUN apt-get update && apt-get install -y --allow-unauthenticated nodejs

COPY . .

RUN bundle install
RUN rails db:migrate

EXPOSE 3000

CMD rails s