FROM node:20.10.0-alpine3.18
WORKDIR /app

COPY package*.json ./
RUN npm install
COPY . .
RUN addgroup -S adm_app && adduser -S vitor -G adm_app
RUN chown -R vitor:adm_app /app
USER vitor

EXPOSE 8080
CMD [ "node", "server.js" ]