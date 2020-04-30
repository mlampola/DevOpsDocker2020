FROM ruby:2.6.0-alpine
WORKDIR /usr/app
COPY . .
EXPOSE 3000
RUN apk add --update nodejs nodejs-npm build-base sqlite sqlite-dev tzdata
RUN bundle install
# Production
#RUN rails db:migrate RAILS_ENV=production
#RUN rake assets:precompile
#CMD RAILS_LOG_TO_STDOUT=true rails s -e production
# Development
RUN rails db:migrate
CMD rails s

