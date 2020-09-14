FROM node
EXPOSE 5000

ADD frontend-example-docker .

RUN apt-get update && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x
RUN apt install -y nodejs
RUN node -v && npm -v
RUN npm install
CMD npm start
