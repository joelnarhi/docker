FROM node
WORKDIR /app
ADD frontend-example-docker /app
RUN apt-get update &&  apt-get install curl -y && \
    curl -sL https://deb.nodesource.com/setup_10.x && \
    apt install -y nodejs && \
    node -v && npm -v && \
    npm install && \
    npm install -g serve && \
    apt-get purge -y --autoremove curl && \
    rm -rf /var/lib/apt/lists/*
EXPOSE 5000
CMD npm start
