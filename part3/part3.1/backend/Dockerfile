FROM node
WORKDIR /app
ADD backend-example-docker /app
RUN apt-get update && apt-get install curl -y && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt install -y nodejs && \
    npm install && \
    apt-get purge -y --autoremove curl && \
    rm -rf /var/lib/apt/lists/*
ENV FRONT_URL=192.168.0.117
CMD npm start
