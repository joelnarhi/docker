FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install curl -y
COPY website.sh .
RUN chmod +x ./website.sh
CMD ["./website.sh"]
