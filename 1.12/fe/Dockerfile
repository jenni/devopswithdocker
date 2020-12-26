# frontend
FROM node:15.5-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY src src
COPY util util
COPY config.js config.js
COPY webpack.config.js webpack.config.js

EXPOSE 5000

ENV API_URL http://localhost:8000

CMD npm start