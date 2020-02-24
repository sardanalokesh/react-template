FROM node:13.8.0-alpine3.11
RUN npm i -g json-server
COPY ./support/dev/json-server/db.json /db.json
COPY ./support/dev/json-server/routes.json /routes.json
EXPOSE 3000
CMD [ "json-server", "-w", "db.json", "-r", "routes.json", "-H", "0.0.0.0" ]
