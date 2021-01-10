FROM ubuntu:16.04
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
WORKDIR /frontend
COPY /frontend-example-docker . 
EXPOSE 5000
CMD npm start
