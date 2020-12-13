FROM node:14-alpine3.10

WORKDIR /client

COPY package.json /client

COPY yarn.lock /client

RUN yarn global add @quasar/cli

RUN npm install 

COPY . /client
