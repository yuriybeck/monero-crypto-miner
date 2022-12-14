FROM ubuntu:20.04

WORKDIR /app
COPY . /app

RUN apt-get -y update && apt-get -y upgrade && apt-get -y install wget vim
RUN wget https://github.com/xmrig/xmrig/releases/download/v6.18.0/xmrig-6.18.0-focal-x64.tar.gz
RUN tar xvzf xmrig-6.18.0-focal-x64.tar.gz
RUN cp -a /app/config /app/xmrig-6.18.0/config.json

CMD ["/app/xmrig-6.18.0/xmrig", "--daemon", "--log-file=/app/run.log"]