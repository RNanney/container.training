FROM ruby:slim
RUN apt-get update && apt-get install -y build-essential curl
RUN gem install sinatra
RUN gem install thin
ADD hasher.rb /
CMD ["ruby", "hasher.rb"]
EXPOSE 80
