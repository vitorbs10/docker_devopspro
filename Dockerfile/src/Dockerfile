FROM node:23-alpine3.19
EXPOSE 8080
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . . 
ENTRYPOINT [ "node","server.js" ]