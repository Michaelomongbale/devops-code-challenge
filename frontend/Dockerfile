FROM node:14-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY package*.json ./

RUN npm install && npm install chokidar

RUN npm install react-scripts -g

COPY . ./

EXPOSE 3000

CMD ["npm", "start"]

