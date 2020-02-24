FROM node:13.8.0-alpine3.11

COPY package.json /app/package.json
WORKDIR /app
RUN npm i

COPY ./public /app/public
COPY ./src /app/src
COPY tsconfig.json /app/tsconfig.json

EXPOSE 3000
ENTRYPOINT [ "npm", "start" ];
