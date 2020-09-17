FROM ubuntu:latest

EXPOSE 8000
ENV FRONT_URL=http://192.168.99.100:5000

RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get -y install nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker.git
WORKDIR ./backend-example-docker
RUN npm install
CMD ["npm", "start"]
