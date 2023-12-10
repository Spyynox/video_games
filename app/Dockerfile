FROM node:21-alpine3.17

WORKDIR /usr/src/app/video_games

COPY package.json .

RUN npm install
RUN mkdir node_modules/.cache && chmod -R 777 node_modules/.cache

COPY . .

EXPOSE 3000

CMD ["npm", "start"]