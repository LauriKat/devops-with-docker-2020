FROM ubuntu:18.04
RUN apt-get update && apt-get install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
RUN apt-get update && apt-get install -y nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker
WORKDIR /backend-example-docker
EXPOSE 8000
RUN npm install 
CMD ["env", "FRONT_URL=http://localhost:5000", "npm", "start"]
