FROM ubuntu:18.04
RUN apt-get update && apt-get install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
RUN apt-get update && apt-get install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker
WORKDIR /frontend-example-docker
EXPOSE 5000
RUN npm install 
CMD ["env", "API_URL=http://localhost:8000", "npm", "start"]

