FROM        node:alpine

ARG         PACKAGES=nano

RUN         apk update && apk add $PACKAGES

WORKDIR     /var/www
COPY        package*.json ./
     
RUN         npm install

COPY        . ./
EXPOSE      8080

ENTRYPOINT  ["npm", "start"]