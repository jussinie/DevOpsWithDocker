FROM ubuntu:16.04
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
WORKDIR /backend
COPY /backend-example-docker .
RUN npm install 
EXPOSE 8000
CMD npm start
