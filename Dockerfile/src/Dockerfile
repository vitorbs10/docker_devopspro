FROM ubuntu
EXPOSE 8080
RUN apt-get update && apt-get install -y curl &&  \
    curl -fsSL https://deb.nodesource.com/setup_23.x -o nodesource_setup.sh &&\
    bash nodesource_setup.sh &&\
    apt-get install -y nodejs
WORKDIR /app
COPY . .
RUN npm install 
ENTRYPOINT [ "node","server.js" ]