FROM node:13-alpine
ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PASSWORD=password

RUN mkdir -p /home/app

COPY . /home/app

RUN npm install:13-alpine

CMD ["node","server.js"]