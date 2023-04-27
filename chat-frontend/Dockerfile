FROM node:17-alpine

ARG TZ=UTC
ENV TZ=Asia/Yangon

RUN apk update && \
    apk add --no-cache python3 make g++

COPY package*.json ./

RUN npm install

WORKDIR /var/www