# JS backend project
FROM node:15.5-alpine

WORKDIR /usr/app

COPY package*.json ./
RUN npm install

COPY server server
COPY index.js index.js
COPY config.js config.js
COPY logs.txt logs.txt

EXPOSE 8000

ENV FRONT_URL localhost:5000

CMD node index.js