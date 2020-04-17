FROM ubuntu:16.04
RUN apt-get -y update && apt-get -y upgrade && apt-get -y install curl
WORKDIR /usr/app
COPY start.sh .
RUN chmod +x ./start.sh
CMD ["./start.sh"]
