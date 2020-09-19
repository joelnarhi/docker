FROM node
ENV FRONT_URL=192.168.0.117
ADD backend-example-docker .

RUN apt-get update && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
CMD npm start
