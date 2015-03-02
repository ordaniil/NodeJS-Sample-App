FROM ubuntu:latest

RUN apt-get -y update
RUN apt-get -y install nodejs
RUN apt-get -y install npm
RUN npm install express -g

ADD . /src

RUN cd /src; npm install

EXPOSE 8080
CMD ["nodejs", "app.js"]
